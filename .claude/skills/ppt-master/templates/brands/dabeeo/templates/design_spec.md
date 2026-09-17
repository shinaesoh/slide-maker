---
brand_id: dabeeo
kind: brand
summary: dabeeo 코퍼레이트 아이덴티티 — 공공사업 제안서, 사업 소개, 기술 발표, 사내 보고
keywords: [dabeeo, 다비오, navy, corporate, korean, gis, 공공, 제안서]
primary_color: "#192A67"
---

# dabeeo Brand Specification

> Identity-only preset. 고정 페이지 로스터 없음 — 아래 제약 안에서 페이지를 자유롭게 구성합니다.
> 2026-09 작성. 색상 토큰은 사내 제품 **Dabeeo Change Cloud**의 디자인 토큰
> (`tailwind.config.js`)에서 가져왔고, 네이비는 공식 로고 워드마크 색상과 대조했습니다.
> 전사 CI 규정 문서와의 대조는 아직 이루어지지 않았습니다 — 아래 Provenance 표기를 확인하세요.

## I. Brand Overview

| Property | Value |
|---|---|
| Brand Name | dabeeo (다비오) |
| Tagline | Reading and Interpreting the Earth |
| Use Cases | 공공사업 제안서, 사업/회사 소개, 기술 발표, 사내 보고 |
| Tone | 절제된 기술 신뢰형 — 공공 발주처를 상정한 사실 중심 서술, 장식 최소화 |

## II. Color Scheme

| Role | HEX | Provenance |
|---|---|---|
| primary | #192A67 | product-token — `navy.DEFAULT`. 공식 로고 워드마크와 동일 계열로 확인 |
| accent | #1E57DC | product-token — `brand.DEFAULT`. 링크·강조·주요 데이터 계열 |
| secondary | #27C4D5 | product-token — `cyan.DEFAULT`. 보조 강조, 차트 2계열 |
| surface | #DCE7F4 | product-token — `bluegray.DEFAULT`. 표 헤더·박스 배경 |
| text | #222222 | product-token — `ink.22`. 본문 잉크 |
| bg | #FFFFFF | fact — 콘텐츠 캔버스 |
| cover | #192A67 | inferred — 로고 다크 버전 배경이 네이비 단색이라 표지/간지에 동일 적용 |

**적용 규칙**: 네이비는 구조색(표지·간지·헤더·타이틀), 브랜드 블루는 강조 1순위(핵심 수치·링크·주요 계열),
시안은 보조 강조로 **페이지당 블루+시안 2색까지**만. 블루그레이는 면(표 헤더, 박스)에만 쓰고 글자색으로 쓰지 않습니다.
중성색: 보조 텍스트 `#444444`, 흐린 텍스트 `#777777`, 헤어라인 `#EAEAEA`.

> ⚠️ **Provenance 주의**: `product-token`으로 표기된 값은 사내 제품 UI의 디자인 토큰입니다.
> 전사 CI 규정집에 별도 지정 값이 있다면 그쪽이 우선하며, 확인 후 이 표를 갱신하고
> `brands_index.json`의 `primary_color`도 함께 고쳐야 합니다.

## III. Typography

| Role | Family | Weight |
|---|---|---|
| title | Pretendard | 700 (SemiBold 600까지 허용) |
| body | Pretendard | 400 |
| kpi/label | Pretendard | 600 |

저장소 전역 Pretendard 락을 따릅니다 — 위계는 서체를 바꾸지 않고 **굵기와 크기**로만 만듭니다.
타이틀 자간 -0.02em, 본문 -0.01em. 숫자는 가능한 경우 tabular figures.
영문 고유명사 `dabeeo`는 **항상 소문자**로 표기합니다.

## IV. Logo

- 파일 (이 design_spec.md 기준 상대경로):
  - `../images/dabeeo-wordmark-navy.png` — 흰 배경용 기본 락업
  - `../images/dabeeo-wordmark-white.png` — 네이비 등 어두운 면 위
  - `../images/dabeeo-lockup-navy.png` — 워드마크 + 태그라인, 흰 배경용
  - `../images/dabeeo-lockup-white.png` — 워드마크 + 태그라인, 어두운 면 위
- 사용: 표지는 태그라인 포함 락업, 본문 페이지는 워드마크만 우상단 소형 배치
- 여백: 워드마크 높이의 0.5배 이상을 사방 클리어스페이스로 확보
- 금지: 임의 색상 변경, 세로 배치, 그림자·외곽선 추가, 비율 왜곡

> ⚠️ **이미지 파일 미포함 상태입니다.** 필요한 파일과 규격은 `../images/README.md`를 보세요.
> 파일을 넣기 전까지 로고가 들어가는 레이아웃은 자리만 잡고 비워 둡니다.

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
