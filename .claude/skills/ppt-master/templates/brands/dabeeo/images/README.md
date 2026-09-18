# dabeeo 로고 자산

## 들어 있는 파일

| 파일명 | 규격 | 쓰이는 곳 | 출처 |
|---|---|---|---|
| `dabeeo-wordmark-white.png` | 1531×342 RGBA | 네이비 표지·간지 등 어두운 면 | `decks/dabeeo_business/images/ending-wordmark.png` 원본 그대로 |
| `dabeeo-wordmark-navy.png` | 1531×342 RGBA | 흰 배경 본문 페이지 우상단 | 위 파일의 **알파 마스크를 그대로 두고 채움색만** `#192A67`로 변경 |

> 네이비 버전은 글리프를 다시 그리거나 트레이싱한 것이 아니라 동일한 마스크의 색만 바꾼 것이라
> 형태가 원본과 픽셀 단위로 같습니다. 공식 가이드의 두 컬러웨이(밝은 면=네이비 / 어두운 면=화이트)에 해당합니다.

## 아직 없는 파일

태그라인이 붙은 락업 2종입니다. 태그라인의 서체·자간·워드마크와의 간격을 제가 임의로 정하면
공식 락업과 달라지므로 **원본 파일이 필요합니다.**

| 파일명 | 내용 |
|---|---|
| `dabeeo-lockup-navy.png` | 워드마크 + `Reading and Interpreting the Earth`, 네이비 |
| `dabeeo-lockup-white.png` | 워드마크 + 태그라인, 흰색 |

규격: PNG 투명 배경(RGBA), 가로 900px 이상. 넣은 뒤
[`../templates/design_spec.md`](../templates/design_spec.md)의 IV. Logo 절에서 "미포함" 표기를 지우세요.

## 주의

- 워드마크를 직접 그리거나 스크린샷을 잘라 쓰지 마세요. `dabeeo`는 커스텀 레터링입니다
- 이 저장소는 **public**입니다. 고객사 로고, 제안서 실물, 미공개 제품 화면은 넣지 마세요
