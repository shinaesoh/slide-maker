# Windows 설치 가이드

Windows PC에 Slide Maker를 설치하는 순서입니다. 처음부터 끝까지 10~15분 정도 걸립니다.

준비물은 **Python**과 **Git** 둘뿐이고, 나머지는 선택입니다.

---

## 1단계 — Python 설치 (필수)

1. **[python.org/downloads](https://www.python.org/downloads/)** 에서 **Python 3.10 이상** 설치 파일을 받습니다.

2. **⚠️ 설치 화면 맨 아래 "Add python.exe to PATH"를 반드시 체크하세요.** Windows에서 가장 흔한 실수이고, 이걸 놓치면 이후 모든 단계가 실패합니다.

3. 설치가 끝나면 시작 메뉴에서 **PowerShell**을 열어 확인합니다.

   ```powershell
   python --version
   ```

   `Python 3.12.x` 같은 표시가 나오면 정상입니다. "Python was not found"가 뜨거나 Microsoft Store가 열리면 아래 [문제 해결](#문제-해결)을 보세요.

> Anaconda·Miniconda로 설치한 Python도 됩니다. `python --version`이 3.10 이상이면 무방합니다.

---

## 2단계 — Git 설치 (필수)

[git-scm.com/downloads](https://git-scm.com/downloads)에서 받아 설치합니다. 설치 옵션은 전부 기본값으로 두면 됩니다.

```powershell
git --version
```

버전이 표시되면 정상입니다.

> ZIP으로 받아도 동작은 하지만, Git으로 받아야 나중에 `git pull` 한 줄로 업데이트할 수 있습니다. 사내 배포에서는 Git 설치를 권장합니다.

---

## 3단계 — 저장소 받기

내 문서 폴더 등 경로에 **한글과 공백이 없는** 위치를 권장합니다. 일부 변환 스크립트가 한글 경로에서 문제를 일으킵니다.

```powershell
cd C:\Users\$env:USERNAME\Documents
git clone https://github.com/shinaesoh/slide-maker.git
cd slide-maker
```

---

## 4단계 — 가상환경 만들고 의존성 설치

패키지를 전역 Python이 아니라 프로젝트 전용 가상환경(venv)에 넣습니다. 회사 PC에서 돌아가는 다른 파이썬 작업과 버전이 충돌하지 않게 하기 위해서입니다.

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

활성화에 성공하면 프롬프트 앞에 `(.venv)`가 붙습니다. 마지막에 `Successfully installed ...`가 나오면 완료입니다.

> `Activate.ps1` 실행이 막히면 → 아래 [PowerShell 스크립트 실행 차단](#powershell에서-스크립트-실행이-차단됩니다)을 보세요.
> `pip`을 못 찾으면 → `python -m pip install -r requirements.txt`로 실행하세요.

**터미널을 새로 열 때마다 활성화가 필요합니다.**

```powershell
cd C:\Users\$env:USERNAME\Documents\slide-maker
.venv\Scripts\Activate.ps1
```

---

## 5단계 — 설치 확인

venv가 활성화된 상태에서:

```powershell
python -c "import pptx, pymupdf, PIL, numpy, flask; print('핵심 의존성 정상')"
```

`핵심 의존성 정상`이 출력되면 됩니다. 오류가 나면 [문제 해결](#문제-해결)로.

> 스크립트나 에이전트가 `import fitz`를 쓰면 "The `fitz` API is deprecated" 경고가 뜰 수 있습니다. **경고일 뿐 오류가 아니며** 동작에는 문제가 없습니다. `fitz`와 `pymupdf`는 같은 패키지입니다.

---

## 6단계 — 에이전트에서 열고 테스트

**반드시 venv가 활성화된 터미널에서 에이전트를 실행하세요.** 그래야 스크립트가 venv의 Python을 씁니다.

- **Claude Code** (권장) — 활성화된 PowerShell에서 `claude` 실행
- **Cursor · VS Code + Copilot** — File → Open Folder로 `slide-maker` 폴더를 열고, 통합 터미널에서 활성화

에이전트 채팅에 이렇게 입력해 봅니다.

```
표지, 본문 1장, 마무리로 구성된 3페이지짜리 테스트 PPT를 만들어줘. 주제는 "Hello World".
```

`projects\<프로젝트명>\exports\` 아래에 `.pptx`가 생기고 PowerPoint에서 열리면 설치 완료입니다.

---

## 7단계 (선택) — 있으면 좋은 것들

Python과 의존성만으로 덱 생성은 전부 동작합니다. 아래는 필요할 때만 설치하세요.

| 항목 | 이럴 때 필요 | 설치 방법 | 확인 |
|---|---|---|---|
| **Pretendard 폰트** | 만든 덱을 이 PC에서 정상적으로 보고 싶을 때. PPTX는 폰트를 내장하지 않으므로 덱을 여는 PC마다 설치가 필요합니다 | `.claude\skills\ppt-master\assets\fonts\Pretendard\` 폴더의 폰트 파일을 전체 선택 → 우클릭 → **설치** | PowerPoint 폰트 목록에 `Pretendard` |
| **Node.js** | AI 이미지 생성(Codex CLI)이나 수출 PPTX 검증(OfficeCLI)을 쓸 때 | [nodejs.org](https://nodejs.org/) LTS 설치 | `node --version` |
| **Pandoc** | `.doc` `.odt` `.rtf` `.tex` 같은 구형 포맷을 변환할 때. `.docx` `.html` `.epub` `.ipynb`는 Python만으로 됩니다 | [pandoc.org](https://pandoc.org/installing.html)에서 `.msi` | `pandoc --version` |

---

## 업데이트

```powershell
cd C:\Users\$env:USERNAME\Documents\slide-maker
git pull
```

의존성 목록이 바뀐 경우에는 활성화 후 `pip install -r requirements.txt`를 한 번 더 실행하세요.

내 작업물이 들어 있는 `projects\` 폴더는 `.gitignore`에 포함되어 있어 `git pull`로 덮어써지지 않습니다.

---

## 문제 해결

### `python`을 찾을 수 없거나 Microsoft Store가 열립니다

**원인**: Python이 PATH에 없습니다.

**해결 1** — Python 설치 파일을 다시 실행 → **Modify** → **"Add Python to environment variables"** 체크

**해결 2** — PATH에 직접 추가
1. PowerShell에서 `where python`으로 실제 경로를 확인합니다 (예: `C:\Users\사용자명\AppData\Local\Programs\Python\Python312\python.exe`)
2. 시작 메뉴에서 "환경 변수" 검색
3. `Path` → **편집** → 위에서 확인한 **폴더**와 그 아래 `Scripts` 폴더를 추가
   ```
   C:\Users\사용자명\AppData\Local\Programs\Python\Python312
   C:\Users\사용자명\AppData\Local\Programs\Python\Python312\Scripts
   ```
4. 확인을 누른 뒤 **PowerShell을 다시 여세요**

**해결 3** — `python` 대신 `py`를 써보세요.

### `python3` 명령이 실패합니다 (exit 49 / Microsoft Store가 열림)

python.org 설치 파일은 `python.exe`만 설치하고 `python3.exe`는 만들지 않습니다. **`python3`를 `python`으로 바꿔서** 실행하세요. 에이전트도 대개 알아서 `python`으로 바꿔 진행합니다.

### PowerShell에서 스크립트 실행이 차단됩니다

`Activate.ps1`을 실행할 때 "running scripts is disabled" 오류가 나면, 둘 중 하나를 쓰세요.

```powershell
# 방법 A — 정책을 한 번만 바꿉니다 (현재 사용자만, 관리자 권한 불필요)
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

```powershell
# 방법 B — 정책을 건드리지 않고 배치 파일로 활성화
.venv\Scripts\activate.bat
```

### `ModuleNotFoundError`가 납니다

venv 활성화를 안 한 상태로 실행했을 가능성이 가장 큽니다. 프롬프트 앞에 `(.venv)`가 있는지 확인하고, 없으면 `.venv\Scripts\Activate.ps1`을 먼저 실행하세요.

활성화했는데도 난다면 pip이 다른 Python에 설치한 경우입니다. `python -m pip install -r requirements.txt`로 다시 설치하세요.

### `import fitz`가 실패합니다

1. pip 업그레이드: `python -m pip install --upgrade pip`
2. 미리 빌드된 wheel 사용: `pip install PyMuPDF --only-binary :all:`
3. 그래도 안 되면 [Visual C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/) 설치

### `pip install`이 권한 오류로 실패합니다

venv를 쓰면 보통 발생하지 않습니다. venv 없이 전역 설치 중이라면:

```powershell
pip install --user -r requirements.txt
```

### `pip install`이 네트워크 문제로 실패합니다

사내망 프록시를 거쳐야 하는 경우:

```powershell
pip install -r requirements.txt --proxy http://프록시주소:포트
```

---

## 그래도 안 되면

- 📖 [FAQ](./faq.md)
- 🐛 [이 저장소의 Issues](https://github.com/shinaesoh/slide-maker/issues) — Python 버전, Windows 버전, 전체 오류 메시지를 함께 남겨주세요
