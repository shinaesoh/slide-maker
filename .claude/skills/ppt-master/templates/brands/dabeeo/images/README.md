# dabeeo 로고 자산 — 넣어야 할 파일

이 폴더는 아직 비어 있습니다. 아래 4개 파일을 **정확히 이 이름으로** 넣으면
[`../templates/design_spec.md`](../templates/design_spec.md)의 로고 참조가 그대로 동작합니다.

| 파일명 | 내용 | 쓰이는 곳 |
|---|---|---|
| `dabeeo-wordmark-navy.png` | `dabeeo` 워드마크, 네이비(`#192A67`) | 흰 배경 본문 페이지 우상단 |
| `dabeeo-wordmark-white.png` | `dabeeo` 워드마크, 흰색 | 네이비 표지·간지 |
| `dabeeo-lockup-navy.png` | 워드마크 + `Reading and Interpreting the Earth`, 네이비 | 흰 배경 표지 |
| `dabeeo-lockup-white.png` | 워드마크 + 태그라인, 흰색 | 네이비 표지 |

## 규격

- **형식**: PNG, 투명 배경(RGBA). SVG가 있으면 SVG를 함께 넣고 PNG도 유지하세요 — 변환기는 PNG 경로를 씁니다
- **해상도**: 가로 **900px 이상** 권장. 표지에서 크게 쓰므로 200px대 이미지는 인쇄·확대 시 깨집니다
- **여백**: 글리프 바깥 여백은 최소로 잘라내세요. 클리어스페이스는 레이아웃에서 계산합니다

## 주의

- 스크린샷을 잘라 만들거나 워드마크를 직접 그려서 넣지 마세요. `dabeeo`는 커스텀 레터링이라
  재현하면 실제 CI와 어긋납니다. **반드시 공식 원본 파일**을 사용하세요
- 이 저장소는 **public**입니다. 로고·브랜드 컬러 외에 고객사 로고, 제안서 실물,
  미공개 제품 화면은 절대 넣지 마세요

파일을 넣은 뒤에는 `design_spec.md`의 IV. Logo 절에 있는 "이미지 파일 미포함 상태" 경고문을 지우세요.
