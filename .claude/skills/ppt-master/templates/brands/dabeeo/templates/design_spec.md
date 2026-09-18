---
brand_id: dabeeo
kind: brand
summary: dabeeo 코퍼레이트 아이덴티티 — 공공사업 제안서, 사업 소개, 기술 발표, 사내 보고
keywords: [dabeeo, 다비오, navy, corporate, korean, gis, 공공, 제안서]
primary_color: "#192A67"
---

# dabeeo Brand Specification

> Identity-only preset. 고정 페이지 로스터 없음 — 아래 제약 안에서 페이지를 자유롭게 구성합니다.
> 2026-09 작성. 색상·서체 토큰은 사내 **dabeeo 디자인 자료**(`dabeeo_design_material`)의 `:root`
> 정의를 그대로 옮긴 것이며, 사내 제품 Dabeeo Change Cloud의 `tailwind.config.js` 및 공식 로고
> 워드마크 색상과 교차 확인했습니다 — 세 출처가 일치합니다.

## I. Brand Overview

| Property | Value |
|---|---|
| Brand Name | dabeeo (다비오) |
| Tagline (EN) | Reading and Interpreting the Earth |
| Tagline (KO) | 지구를 읽고 해석합니다 |
| Use Cases | 공공사업 제안서, 사업/회사 소개, 기술 발표, 사내 보고 |
| Tone | 절제된 기술 신뢰형 — 공공 발주처를 상정한 사실 중심 서술, 장식 최소화 |

## II. Color Scheme

> ⚠️ **저장소 안에 dabeeo 색 기준이 두 벌 있습니다. 이건 그중 범용 쪽입니다.**
>
> | | 이 프리셋 (`brands/dabeeo`) | `decks/dabeeo_business` |
> |---|---|---|
> | 성격 | 범용 아이덴티티 — 제안서·보고·발표 전반 | 기업소개 덱 **전용 스킨** (28페이지 고정 구성) |
> | 파랑 | `#1E57DC` | `#214DC5` |
> | 구조색 | `#192A67` | `#112662` · `#253062` |
> | 출처 | 사내 디자인 자료 `:root` 토큰 + 제품 토큰 (일치) | 실제 제안서에서 추출된 것으로 보임 |
>
> **둘 중 어느 쪽이 전사 CI인지는 확정되지 않았습니다.** 디자인 담당자 확인 전까지 둘을
> 통합하지 않고 용도로 분리해 둡니다. 덱 템플릿을 고르면 SKILL.md Step 4 reconciliation에 따라
> **덱 스킨이 이 표를 덮어씁니다** — 한 덱 안에서 두 기준이 섞이지는 않습니다.
>
> 기업소개 덱을 만들 게 아니라면 이 프리셋을 쓰세요.

사내 디자인 자료의 `:root` 토큰 전체입니다. 토큰명을 그대로 유지했습니다.

| Role | Token | HEX | 용도 |
|---|---|---|---|
| primary | `--navy` | #192A67 | 구조색 — 표지·간지·헤더·타이틀 |
| accent | `--blue` | #1E57DC | 강조 1순위 — 핵심 수치, 링크, 주요 데이터 계열 |
| secondary | `--cyan` | #27C4D5 | 보조 강조 — 차트 2계열, 대비 포인트 |
| surface | `--bluegray` | #DCE7F4 | 표 헤더·박스 면 |
| surface-light | `--bluelight` | #F7F9FF | 옅은 강조 면 |
| deep | `--dark` | #0A1743 | 최심부 네이비 — 풀블리드 표지, 네이비 위 대비 |
| text | `--text-pri` | #222222 | 본문 잉크 |
| text-secondary | `--text-sec` | #444444 | 보조 텍스트 |
| text-muted | `--text-muted` | #777777 | 캡션·주석 |
| bg | `--bg` | #F4F6FB | 문서 배경 (슬라이드 캔버스는 #FFFFFF) |

**Provenance**: 위 10개 값은 전부 사내 디자인 자료의 `:root` 정의 원문이며 추정값이 아닙니다.
`--navy` · `--blue` · `--cyan` · `--bluegray`는 Dabeeo Change Cloud 제품 토큰과도 일치합니다.

**적용 규칙**: 네이비는 구조, 블루는 강조 1순위, 시안은 보조 강조로 **페이지당 블루+시안 2색까지**만.
블루그레이·블루라이트는 면에만 쓰고 글자색으로 쓰지 않습니다. 헤어라인 `#EAEAEA`.

## III. Typography

| Role | Family | Weight |
|---|---|---|
| display | Paperlogy (fallback: Georgia, serif) | 700 |
| title | Pretendard | 700 (SemiBold 600까지 허용) |
| body | Pretendard | 400 |
| kpi/label | Pretendard | 600 |

본문·UI는 Pretendard입니다 — 사내 자료의 `--font` 토큰이 `'Pretendard', -apple-system, BlinkMacSystemFont, sans-serif`이고,
이 저장소의 전역 Pretendard 락과도 일치합니다. 위계는 서체를 바꾸지 않고 **굵기와 크기**로만 만듭니다.
타이틀 자간 -0.02em, 본문 -0.01em. 숫자는 가능한 경우 tabular figures.
영문 고유명사 `dabeeo`는 **항상 소문자**로 표기합니다.

**Paperlogy**는 사내 자료에서 "지구를 읽고 해석합니다", "Reading the Earth" 같은 **대형 문구에만** 쓰이는
디스플레이 서체입니다. 본문·불릿·표에는 쓰지 마세요 — 그 자리는 Pretendard입니다.

- 번들 위치: `.claude/skills/ppt-master/assets/fonts/Paperlogy/` — Thin 100 ~ Black 900 전 9종
- 라이선스: SIL OFL 1.1, Copyright © 2024 PT& — 폰트 파일 내 name table로 확인. 같은 폴더의 `LICENSE.txt` 참조
- PPTX는 폰트를 내장하지 않으므로, **덱을 여는 PC마다 Paperlogy 설치가 필요합니다.** 미설치 환경에서는
  Georgia/serif로 대체돼 인상이 크게 달라지므로, 외부 배포용 덱은 Pretendard 700으로 통일하는 편이 안전합니다

> ⚠️ **다국어 덱에는 Paperlogy를 쓰지 마세요.** 한국어와 기본 라틴 문자만 지원합니다.
> 굵기를 9종 전부 번들했지만 굵기와 언어 커버리지는 무관합니다 — 9종 모두 같은 글리프 세트입니다.
>
> | 문자 | Paperlogy | Pretendard |
> |---|---|---|
> | 한글 음절 | 100% | 100% |
> | 라틴 기본(영어) | 100% | 100% |
> | 라틴 확장-A (폴란드·체코·터키) | 7% | 99% |
> | 라틴 확장-B (베트남 등) | 1% | 99% |
> | 키릴 (러시아) | 0% | 99% |
> | 그리스 | 0% | 84% |
> | 히라가나·가타카나 (일본) | 0% | 94~98% |
> | CJK 한자 (중국) | 0% | 0% |
>
> 영어 외 언어가 섞이면 **Pretendard로 조판**하세요. 중국어·일본어 한자는 두 폰트 모두 미지원이라
> 별도 폰트(Noto Sans CJK 등)가 필요합니다.

## IV. Logo

- 파일 (이 design_spec.md 기준 상대경로):
  - `../images/dabeeo-wordmark-navy.png` (1531×342) — 흰 배경용 기본
  - `../images/dabeeo-wordmark-white.png` (1531×342) — 네이비 등 어두운 면 위
  - `../images/dabeeo-lockup-navy.png` — 워드마크 + 태그라인, 흰 배경용 **(미포함)**
  - `../images/dabeeo-lockup-white.png` — 워드마크 + 태그라인, 어두운 면 위 **(미포함)**
- 사용: 표지는 태그라인 포함 락업, 본문 페이지는 워드마크만 우상단 소형 배치
- 여백: 워드마크 높이의 0.5배 이상을 사방 클리어스페이스로 확보
- 금지: 임의 색상 변경, 세로 배치, 그림자·외곽선 추가, 비율 왜곡

> 락업 2종은 아직 없습니다. 그때까지 표지는 **워드마크 + 태그라인을 텍스트로 조판**해 대체하고,
> 태그라인은 Paperlogy 700으로 둡니다. 자세한 내용은 `../images/README.md` 참조.

## V. Voice & Tone

- Formality: formal — 합니다체 서술, 개조식 불릿은 명사형 종결
- Person: 무인칭 서술. 발주처를 직접 호칭하지 않습니다
- Emoji: 금지. 느낌표·마케팅 수사도 쓰지 않습니다
- Abbreviations: 기술 용어는 영문 유지(GIS, RMSE, GSD, SaaS), 그 외는 한국어
- 수치는 단위와 기준 시점을 함께 적습니다 ("2024년 기준 1,840km²")

## VI. Icon Style

- Preference: linear — 1.5px 얇은 스트로크. 저장소 번들 Tabler outline 세트 사용
- 아이콘 색은 네이비 또는 브랜드 블루 단색. 다색 아이콘 금지

## VII. Visual Assets

- `../images/` — 워드마크·락업 PNG 4종 (현재 비어 있음)
