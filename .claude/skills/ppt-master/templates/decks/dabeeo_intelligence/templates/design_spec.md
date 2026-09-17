---
deck_id: dabeeo_intelligence
kind: deck
category: brand
summary: 다비오 인텔리전스 기업소개 스타일 — 위성·공간 데이터 AI 기업 브리핑, 기술 신뢰성 설명, 사업화 현황 보고
keywords: [dabeeo, 지구 인텔리전스, 위성영상 AI, 기업소개, 기술신뢰성]
primary_color: "#214DC5"
canvas_format: ppt169
canvas_width: 1280
canvas_height: 720
canvas_viewbox: "0 0 1280 720"
source_canvas_width: 1280
source_canvas_height: 720
source_viewbox: "0 0 1280 720"
replication_mode: fidelity
native_structure_mode: structured
page_count: 28
placeholders:
  01_cover: ["{{TITLE}}", "{{TITLE_2}}", "{{SUBTITLE}}"]
  01a_cover_split: ["{{TITLE}}", "{{TITLE_2}}", "{{SUBTITLE}}", "{{DATE}}"]
  02_toc: ["{{PAGE_TITLE}}", "{{PAGE_NUM}}", "{{TOC_ITEM_1_TITLE}}", "{{TOC_ITEM_1_DESC}}"]
  02_chapter: ["{{CHAPTER_NUM}}", "{{CHAPTER_TITLE}}", "{{CHAPTER_DESC}}"]
  02a_chapter_gradient: ["{{CHAPTER_NUM}}", "{{CHAPTER_TITLE}}", "{{CHAPTER_DESC}}"]
  03_content: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{CONTENT_AREA}}", "{{PAGE_NUM}}"]
  03a_content_fact_table: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03b_content_two_col: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03c_content_three_col: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03d_content_kpi: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03e_content_bullet_hero: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03f_content_grid_cards: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03g_content_matrix: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03h_content_compare: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03i_content_table: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03j_content_process: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03k_content_diagram: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03l_content_timeline: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03m_content_domain_map: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03n_content_chart_trend: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03o_content_chart_compare: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03p_content_chart_composition: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03q_content_chart_dashboard: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03r_content_chart_matrix: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03s_content_chart_roadmap: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  03t_content_image_full: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{CAPTION}}", "{{PAGE_NUM}}"]
  03u_content_credential: ["{{EYEBROW}}", "{{PAGE_TITLE}}", "{{LEAD}}", "{{PAGE_NUM}}"]
  04_ending: ["{{ENDING_SUBTITLE}}", "{{CLOSING_MESSAGE}}"]
---

# Dabeeo Intelligence Deck — Design Specification

> `fidelity` 모드로 `다비오_소개.pptx`(15슬라이드 / 마스터 1 / 레이아웃 17)에서 저작.
> 브랜드 아이덴티티와 페이지 크롬은 원본을 충실히 재현하고, Master/Layout/슬롯 체계와
> 페이지 로스터는 새로 설계했다. 원본 레이아웃 17개는 전부 "챕터 번호만 다른 동일 헤더"
> 계열이었으므로 출력 토폴로지 입력으로 사용하지 않았다.

---

## I. Template Overview

| Property | Value |
| --- | --- |
| **Display Name** | Dabeeo Intelligence Deck |
| **Use Cases** | 기업 소개, 기술 신뢰성 브리핑, 사업화 현황 보고, 투자자·발주처 대상 회사 개요 |
| **Design Tone** | 절제된 기술 브리핑 — 흰 바탕 · 로열블루 위계 · 지구 관측 사진을 한 장씩만 크게 |
| **Theme Mode** | Light — 본문 전 페이지 흰 배경, 표지/간지/클로징만 사진·그라데이션 면 |

한눈에 알아보는 표식: **왼쪽 세로 헤어라인 레일 + 파란 챕터 번호 배지**, 가운데 정렬 3단
헤더(시안 eyebrow → 파란 제목 → 회색 리드), 그리고 하단 전폭 푸터(페이지 번호 · 저작권 ·
워드마크). 사진은 장식으로 흩뿌리지 않고 표지·간지·클로징·전면 이미지 페이지에서만
전면으로 쓴다.

**Anti-mood**(설계 시 배제): 그라디언트 SaaS 대시보드, 아이콘 그리드 인포그래픽,
라운드 카드 남발, 다색 팔레트.

---

## II. Color Scheme

| Role | HEX | Usage |
| --- | --- | --- |
| Primary | `#214DC5` | 제목, 챕터 번호 배지, 주 계열 막대/선, 강조 패널 |
| Deep navy | `#112662` | 표지 부제, 카드 소제목 |
| Eyebrow cyan | `#00B0F0` | 헤더 eyebrow, 태그, 인사이트 바 키라인 |
| Accent sky | `#34A8FD` | 2계열 데이터, 보조 패널 헤더 |
| Link blue | `#1A5FC6` | 간지 보조 설명 |
| Body ink | `#434C61` | 본문 텍스트 |
| Panel | `#F1F5FB` | 카드·표 밴딩 면 |
| Hairline | `#D7DEEC` | 카드 테두리, 그리드 선 |
| Rail / footer | `#BFBFBF` / `#808080` | 좌측 레일, 푸터 문자 |
| Alert / warn | `#E54B4B` / `#FFC000` | 리스크·주의 표기 전용(기본 페이지에서는 미사용) |

**적용 규칙** — 한 페이지에서 계열 색은 최대 3개(`#214DC5` → `#34A8FD` → `#00B0F0`)까지만
쓰고, 그 이상 구분이 필요하면 같은 파랑의 불투명도 단계(0.9 → 0.7 → 0.45)로 내려간다.
원본 덱의 시각 문법이 "파랑 한 계열의 농도 위계"이기 때문이다.

---

## III. Typography

전 페이지 Pretendard 단일 패밀리. 위계는 굵기와 크기로만 만든다.

| Role | Stack | Size |
| --- | --- | --- |
| 표지 제목 | `'Pretendard ExtraBold'` | 88 (분할 표지 62), letter-spacing −4.44 |
| 간지 번호/제목 | `'Pretendard ExtraBold'` | 80, letter-spacing −4.44 |
| 페이지 제목 | `Pretendard` + `font-weight="bold"` | 34.67 |
| Eyebrow | `'Pretendard SemiBold'` | 21.33 |
| 리드 | `Pretendard` | 18.67 |
| 카드 제목 | `'Pretendard SemiBold'` | 19 |
| 본문 | `Pretendard` | 14.67 |
| 푸터·레일 | `'Pretendard ExtraLight'` | 10.67 ~ 13.33 |

Pretendard는 이 머신에 사용자 단위로 설치되어 있고 패키지는 폰트를 포함하지 않는다.
다른 PC에서 열 때는 Pretendard 설치가 필요하다.

---

## IV. Signature Design Elements

- **좌측 레일 + 챕터 배지** — `x=56.89`에서 `y=0..538.22`까지 1.333px 헤어라인, 그 위
  `0,67.11` 56.89×44.21 파란 사각형에 흰 챕터 번호. 레일과 세로 워드마크는 Layout 아톰,
  챕터 번호·챕터 라벨은 장마다 바뀌므로 **Slide-local** `chapter-mark` 그룹이다.
- **3단 중앙 헤더** — eyebrow(y 45.56) → 제목(y 87.11) → 리드(y 140.83), 모두 폭
  1103.83로 `x=103.17`부터. 세 줄 모두 중앙 정렬이 원본의 고유 리듬이다.
- **푸터 밴드** — `y 672..711`. 가운데 저작권 문구, 좌측 페이지 번호, 우측 워드마크
  이미지. 저작권/워드마크는 Layout 아톰, 페이지 번호는 `slide-number` 슬롯.
- **레이아웃 그리드** — 콘텐츠 영역은 `x 88..1200`(폭 1112), `y 224..664`(높이 440).
  3열은 360폭 + 16 거터, 2열은 536폭 + 40 거터, 4열 KPI는 268폭 + 16 거터.
- **이미지 시스템** — 사진은 전면(full-bleed)으로만 쓴다. 표지·간지는 우측에 사진을 두고
  `#FFFFFF` 좌→우 페이드 스크림으로 텍스트 가독 영역을 확보한다. 클로징은 전면 사진 위에
  39.4% 블랙 스크림. 본문 카드 안에 작은 사진을 넣지 않는다.
- **밀도 리듬** — 한 페이지에 주장(제목) 1개, 근거 블록 3~6개. 6개를 넘으면 페이지를
  나눈다. 카드 내부는 소제목 1줄 + 본문 최대 3줄.

---

## V. Page Roster

Master는 전 페이지 공통 `dabeeo-master` / "Dabeeo Intelligence" 하나이며, Master 아톰은
전면 흰 배경 `master-bg` 1개다. 아래 Layout 키가 실제 PowerPoint 레이아웃이 된다.

| File | Layout key | PowerPoint layout name | 설명 |
| --- | --- | --- | --- |
| `01_cover.svg` | `cover` | Cover | 우측 지구 사진 + 좌→우 흰 페이드, 88px 2행 브랜드 타이틀과 법인명. 표지 고정 구도 |
| `01a_cover_split.svg` | `cover_split` | Cover (Split) | 좌 카피 / 우 사진 밴드(608×306, 원본 비율 유지) 분할 표지. 날짜 줄 포함, 제목 62px |
| `02_toc.svg` | `toc` | Table of Contents | 2열 6항목 목차. 연번은 28% 불투명 대형 숫자, 항목마다 헤어라인 |
| `02_chapter.svg` | `chapter` | Chapter Divider | 원본 간지 재현 — 우측 지구 사진 + 페이드, 80px 챕터 번호/제목, 회전 헤어라인 |
| `02a_chapter_gradient.svg` | `chapter_gradient` | Chapter Divider (Gradient) | 사진 없이 `#214DC5`→`#34A8FD` 전면 그라데이션. 사진 자산이 없을 때의 간지 |
| `03_content.svg` | `content_full` | Content (Full Width) | 표준 헤더 + 자유 콘텐츠 영역 셸. 정해진 구성이 없을 때의 기본 본문 |
| `03a_content_fact_table.svg` | `content_full` | Content (Full Width) | 좌 6행 키/값 팩트 표 + 우 파란 선언 패널. 기업개요·제품개요용 |
| `03b_content_two_col.svg` | `content_two_col` | Content (Two Column) | 색 헤더를 가진 좌우 대칭 패널 2개. 좌우 본문 슬롯 별도 |
| `03c_content_three_col.svg` | `content_three_col` | Content (Three Column) | 번호 메달리온 3주 기둥, 하단 태그 라인. 본문 슬롯 3개 |
| `03d_content_kpi.svg` | `content_full` | Content (Full Width) | 4개 KPI 타일 + 하단 takeaway 바. 숫자 62px |
| `03e_content_bullet_hero.svg` | `content_media_right` | Content (Media Right) | 좌 불릿 4개 + 우 교체 가능한 picture 슬롯 |
| `03f_content_grid_cards.svg` | `content_full` | Content (Full Width) | 3×2 기술 카드 그리드, 카드마다 좌측 4px 액센트 바 |
| `03g_content_matrix.svg` | `content_full` | Content (Full Width) | 버티컬 행 × 기능 열 4×4 매트릭스. 농도로 적합도 표현 |
| `03h_content_compare.svg` | `content_full` | Content (Full Width) | 중립 기준 열 vs 강조된 다비오 열 4행 비교 |
| `03i_content_table.svg` | `content_full` | Content (Full Width) | 4열 5행 데이터 표. **네이티브 PPTX 테이블 마커** + 밴딩 SVG 폴백 |
| `03j_content_process.svg` | `content_full` | Content (Full Width) | 5단계 셰브런 프로세스 + 하단 성과 바. 농도가 단계별로 상승 |
| `03k_content_diagram.svg` | `content_full` | Content (Full Width) | 4층 레이어드 아키텍처, 층마다 모듈 칩 4개 |
| `03l_content_timeline.svg` | `content_full` | Content (Full Width) | 수평 축 위아래 교차 배치 마일스톤 카드 5개 |
| `03m_content_domain_map.svg` | `content_full` | Content (Full Width) | 사업영역 3열, 열마다 항목 칩 5개 |
| `03n_content_chart_trend.svg` | `content_full` | Content (Full Width) | 2계열 라인 추이. **네이티브 차트 마커(line)** + 인사이트 바 |
| `03o_content_chart_compare.svg` | `content_full` | Content (Full Width) | 4항목 2계열 그룹 막대. **네이티브 차트 마커(column)** + 값 라벨 |
| `03p_content_chart_composition.svg` | `content_full` | Content (Full Width) | 구성비 도넛 + 우측 비중 레전드. **네이티브 차트 마커(doughnut)** |
| `03q_content_chart_dashboard.svg` | `content_full` | Content (Full Width) | 상단 KPI 3타일 + 하단 누적 막대. **네이티브 차트 마커(column)** |
| `03r_content_chart_matrix.svg` | `content_full` | Content (Full Width) | 2×2 포지셔닝 사분면, 가중 버블. 벡터 전용(네이티브 마커 없음) |
| `03s_content_chart_roadmap.svg` | `content_full` | Content (Full Width) | 6구간 스케일 위 3트랙 스윔레인 로드맵. 벡터 전용 |
| `03t_content_image_full.svg` | `content_image_full` | Content (Full Image) | 상단 전면 이미지 밴드(높이 452) + 하단 캡션 블록. 좌측 레일 없음 |
| `03u_content_credential.svg` | `content_full` | Content (Full Width) | 인증 배지 3개 + 하단 신뢰성 서술 3줄 |
| `04_ending.svg` | `ending` | Closing | 블랙 Layout 배경 위 지구 사진 60.6% 합성(= 원본 39.4% 블랙 스크림과 동일), 워드마크 워터마크, 사인오프 2행 |

### Layout 키 정리

11개 Layout 키가 28개 페이지를 담당한다. 같은 키를 쓰는 페이지들은 고정 Layout 아톰과
슬롯 id/타입/인덱스/기본 bounds가 완전히 동일하며, 차이는 전부 Slide-local 콘텐츠다.

| Layout key | 슬롯 구성 | 사용 페이지 수 |
| --- | --- | --- |
| `cover` | title, subtitle | 1 |
| `cover_split` | title, subtitle, body(1) | 1 |
| `toc` | title, slide-number | 1 |
| `chapter` | body(1), title, body(2) | 1 |
| `chapter_gradient` | body(1), title, body(2) | 1 |
| `content_full` | body(1) eyebrow, title, body(2) lead, slide-number | 17 |
| `content_two_col` | + body(3), body(4) | 1 |
| `content_three_col` | + body(3), body(4), body(5) | 1 |
| `content_media_right` | + body(3), picture(6) | 1 |
| `content_image_full` | picture(6), body(1), title, body(2), slide-number | 1 |
| `ending` | subtitle, title | 1 |

`03r` / `03s`는 `content_full` 키를 쓰되 리드 슬롯을 비워 두고 쓰는 것을 권장한다. 같은 키를
공유하는 페이지는 슬롯 집합이 완전히 동일해야 하므로 슬롯 자체는 모두 존재한다.

---

## VI. Assets

템플릿 자산은 6개이고, 나머지 60여 개 원본 이미지는 샘플 콘텐츠로 판단해 제외했다.

> **배포 상태** — 이 저장소는 public이므로 `cover-earth.png` / `chapter-earth.png` /
> `ending-earth.jpg` 세 장은 **플레이스홀더**로 들어 있다(원본은 제3자 스톡 성격이라
> 재배포하지 않는다). 사용권이 있는 이미지로 교체하는 방법은
> [`../images/README.md`](../images/README.md)에 있다. 파일명과 픽셀 크기는 바꾸지 않는다.

| File | Size | Usage |
| --- | --- | --- |
| `dabeeo-logo-footer.png` | 58×13 | 전 본문 페이지 우하단 워드마크(Layout 아톰) |
| `cover-earth.png` ⚠️ | 1066×536 | `01_cover` 우측 사진, `01a_cover_split` 우측 전면 사진 |
| `chapter-earth.png` ⚠️ | 863×434 | `02_chapter` 우측 사진, `03e` picture 슬롯 기본값 |
| `chapter-hairline.png` | 1106×3 | `02_chapter` 회전 헤어라인(불투명도 0.55) |
| `ending-earth.jpg` ⚠️ | 1280×640 | `04_ending` 전면 배경, `03t` picture 슬롯 기본값 |
| `ending-wordmark.png` | 1531×342 | `04_ending` 26% 워터마크 |

**이미지 좌표 주의** — 원본은 이 사진들을 `<svg viewBox>` 크롭 래퍼로 감싸 배치했다.
크롭 비율이 동일하도록 좌표를 환산해 평면 `<image>`로 저작했으므로, 프레임을 옮길 때는
비율이 아니라 **환산된 x/width**를 함께 조정해야 한다(예: 표지 `x=214.55 width=1065.55`).

---

## VII. Native Object Policy

데이터 차트 4종(`03n` line · `03o` column · `03p` doughnut · `03q` column)과 데이터 표
1종(`03i`)은 `data-pptx-native` 마커를 달고 있다. 마커는 **휴면 상태**이며
`svg_to_pptx.py --native-objects`로 내보낼 때만 편집 가능한 PowerPoint 차트/표가 된다.
기본 경로는 그려진 SVG 폴백을 그대로 쓴다.

마커 그룹은 의도적으로 `chart` / `table` **placeholder 슬롯이 아니라** 일반
Slide-local 콘텐츠 그룹이다. 네이티브 슬롯 카리어는 `--native-objects` 없이는 바인딩할
수 없어, 기본 내보내기까지 강제로 묶이지 않도록 분리했다.

**팔레트는 메타데이터에만 있다** — 네이티브 내보내기는 SVG 폴백 도형을 버리므로, 폴백을
칠한 색은 PowerPoint 차트로 전달되지 않는다. 각 마커는 `style.colors`(계열 색)와, 필요한
경우 `series[].point_colors`(포인트별 색)로 다비오 팔레트를 **명시**한다. 이 값이 없으면
Office 기본 팔레트(`#4472C4` / `#ED7D31` / `#A5A5A5` …)로 렌더된다.

| 마커 | 지정 방식 | 색 |
| --- | --- | --- |
| `03n` line | `style.colors` | `#214DC5`, `#34A8FD` |
| `03o` column | `style.colors` | `#214DC5`, `#AFC0E8` |
| `03p` doughnut | `series[0].point_colors` | `#214DC5`, `#34A8FD`, `#00B0F0`, `#AFC0E8` |
| `03q` column | `series[0].point_colors` | `#9BAFE5` → `#214DC5` 5단 램프 |
| `03i` table | 셀 `fill` / `color` + `style.border_color` | 헤더 `#214DC5`, 밴딩 `#F1F5FB` |

`03q`의 5단 램프는 SVG 폴백에서 `#214DC5`의 불투명도 0.45→1.0이었다. 네이티브 차트에는
포인트별 불투명도가 없으므로 **흰 바탕에 합성한 solid 색으로 환산**해 양쪽이 같게 만들었다.
차트 색을 바꿀 때는 폴백 도형과 마커 메타데이터를 **반드시 함께** 수정한다.

네이티브 경로는 편집 우선이라 손실이 있을 수 있다 — 마커 안의 값 라벨, 도넛 중앙 KPI,
축 고정 범위는 정규화되거나 사라질 수 있다. 두 결과를 비교한 뒤 배포한다.
`03r` / `03s`는 PowerPoint 차트로 대응되지 않는 구성이라 벡터 전용으로 남겼다.


---

## VIII. Known Deviations & Notes

1. **클로징 스크림 합성 방식** — 원본은 사진 위에 39.4% 블랙 사각형을 얹었다. 전면 단색
   사각형은 Layout 배경으로 승격되어 Layout 도형보다 먼저 그려져야 하므로, 동일한 결과가
   나오도록 **검정 Layout 배경 + 사진 불투명도 0.606**으로 뒤집어 저작했다(합성 결과 동일).
2. **엔딩 워드마크 1개** — 원본은 같은 워드마크를 26% 전체 + 부분 크롭 하이라이트로 두 번
   얹었다. 크롭 하이라이트는 생략하고 26% 한 장만 남겼다. 이 템플릿의 유일한 시각적 단순화다.
3. **이미지 업스케일 경고** — `ending-earth.jpg`(1280×640)를 1430px 폭으로 늘려 쓴다.
   원본 덱이 크롭 래퍼로 같은 확대를 했기 때문이며, 품질 검사기는 이를 경고로만 표시한다.
4. **`Pretendard Bold` 안전 목록 누락** — `svg_quality_checker.py`의 `PPT_SAFE_FONTS`에
   Light/Medium/SemiBold/ExtraBold 등은 있으나 `pretendard bold`만 빠져 있다. 이 템플릿은
   우회해서 `Pretendard` + `font-weight="bold"`로 저작했다. 저장소 차원의 목록 보정은 별도
   판단 사항이다.
