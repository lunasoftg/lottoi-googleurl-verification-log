# [세계 최초! 로또아이(LOTTOi)](https://www.lottoi.kr) 공개 검증 로그 저장소
*(LOTTOi Public Verification Log Repository)*

---

이 저장소는 **[로또아이(LOTTOi)](https://www.lottoi.kr)** 서비스의 **결과 공개 검증 시스템**을 구성하는 핵심적인 **외부 기준 로그(Verification Log)** 저장소입니다. 

로또아이는 2025년 2월 8일부터 세계 최초로 외부 플랫폼(Google/GitHub) 연동형 검증 구조를 통해 운영 이력의 투명성을 증명하고 있습니다.

---

## 📋 무엇을 기록하나요?

로또아이는 회원이 생성한 번호를 로또 복권 구매 마감 직후인 **토요일 20:00부터 추첨 전(20:35)**까지 **외부 문서(Google 공개 문서)** 형태로 일괄 기록합니다. 

이 Google 문서는 회차별로 고유한 URL을 가지며, 다음 정보가 제3자 시스템(Google)에 의해 기록됩니다.

- 문서의 **최초 생성 시점** (추첨 이전 생성 여부 확인)
- 데이터 저장 이후의 **변경 이력**
- 모든 변경의 **구체적인 시간 순서**

---

## 🔗 이 저장소의 역할 (External Anchor)

이 저장소는 데이터를 직접 보증하는 공간이 아니라, 각 회차의 **Google 공개 문서 URL이 추첨 이전에 이미 외부에 존재했는지**를 기록하고 공개하기 위한 **외부 기준 로그(Anchor)** 역할을 합니다.

> **“이 URL이 언제부터 전 세계에 공개되어 있었는가?”**  

를 외부 시스템(GitHub)에서 다시 한번 공증함으로써, 운영자가 사후에 임의로 문서를 교체하거나 시간을 조작하는 행위를 기술적으로 무력화합니다.

---

## ✅ 무엇을 검증할 수 있나요?

누구나 본 저장소의 로그와 Google 문서를 대조하여 다음 사항을 검토할 수 있습니다.

1.  **시점의 정당성:** GitHub에 기록된 URL 로그 시점이 추첨 이전인가?
2.  **데이터의 무결성:** Google 문서의 '버전 기록'상 최종 저장 시점이 추첨 시간(20:35) 이전인가?
3.  **변경의 투명성:** 추첨 이후 수정이 발생했다면, 그 내용과 시점이 은폐 없이 공개되어 있는가?

이 모든 과정은 [로또아이](https://www.lottoi.kr)가 지향하는 **'조작의 실효성이 없는 투명한 검증 환경'**의 일부입니다.

---

## 📄 공개 검증 백서 (Whitepaper)

로또아이 서비스 전체의 공개 검증 원칙, 운영 기준, 상세 검증 방법에 대한 정보는 아래 백서를 참고해 주세요.

- [**로또아이 결과 공개 검증 백서 (Korean)**](./WHITEPAPER.md)
- [**LOTTOi Public Verification Whitepaper (English)**](./WHITEPAPER.en.md)

---

## 🌐 Public Verification Overview (EN)

This repository serves as an **external verification log** within [LOTTOi](https://www.lottoi.kr)’s public verification system, established on **February 8, 2025**.

It acts as a technical **anchor** by recording when each Google public document URL first existed externally. This allows anyone to verify that records were finalized **before the lottery draw** and ensures that any subsequent changes are fully traceable and cannot be concealed.

For full technical details, please refer to the English Whitepaper linked above.
