# dabeeo_intelligence 이미지 자산

이 폴더의 6개 파일은 `templates/*.svg`에서 `../images/<name>`으로 참조합니다.
**파일명과 픽셀 크기를 바꾸지 마세요** — SVG의 좌표가 이 크기를 전제로 환산돼 있습니다.

## 교체가 필요한 파일 (현재 플레이스홀더)

아래 3개는 파란 그라데이션 플레이스홀더입니다. 이 저장소는 **public**이라 원본
스톡 이미지를 담지 않습니다. 각자 사용권이 있는 이미지로 교체하세요.

| 파일명 | 크기 | 쓰이는 곳 | 필요한 그림 |
|---|---|---|---|
| `cover-earth.png` | 1066×536 | `01_cover` 우측, `01a_cover_split` 우측 밴드 | 가로로 긴 히어로 이미지. 좌측 1/3은 흰 스크림이 덮으므로 주요 피사체를 우측에 |
| `chapter-earth.png` | 863×434 | `02_chapter` 우측, `03e` picture 슬롯 기본값 | 위와 같은 계열의 간지용 이미지 |
| `ending-earth.jpg` | 1280×640 | `04_ending` 전면 배경, `03t` picture 슬롯 기본값 | 전면 배경. 39.4% 검정이 덮이므로 어두워져도 읽히는 것으로 |

교체 후 확인:

```bash
python3 .claude/skills/ppt-master/scripts/svg_quality_checker.py .claude/skills/ppt-master/templates/decks/dabeeo_intelligence/templates --template-mode --format ppt169
```

## 포함된 자산

| 파일명 | 크기 | 쓰이는 곳 |
|---|---|---|
| `dabeeo-logo-footer.png` | 58×13 | 전 본문 페이지 우하단 워드마크 (Layout 아톰) |
| `ending-wordmark.png` | 1531×342 | `04_ending` 26% 워터마크 |
| `chapter-hairline.png` | 1106×3 | `02_chapter` 회전 헤어라인 |

`dabeeo-logo-footer.png`는 58px 폭이라 확대하면 깨집니다. 공식 원본 워드마크가 있으면
같은 이름·같은 비율(약 4.5:1)로 고해상도 파일로 교체하는 편이 좋습니다.
