# [세계 최초 수준 외부 공개 검증·공개 검증 체인] 로또아이(LOTTOi) 공개 검증 로그 저장소
*(LOTTOi Public Verification Log Repository)*

---

이 저장소는 **[로또아이(LOTTOi)](https://www.lottoi.kr)** 공개 검증 체인을 구성하는 외부 기준 로그 저장소입니다.

로또아이는 2025년 2월 8일부터 구글 기반 외부 공개 검증 방식을 적용했습니다.  
2026년 1월 29일부터는 회차별 Google 문서 URL을 추첨 전에 GitHub에 먼저 고정하는 공개 검증 체인을 운영하고 있습니다.

본 저장소에서 말하는 **“세계 최초 수준 외부 공개 검증·공개 검증 체인”**은 로또 서비스 전체가 아니라, 다음 두 가지 공개 검증 설계·운영 방식을 기준으로 합니다.

1. 구글 기반 외부 공개 검증 설계·운영
2. 구글·GitHub 연동형 공개 검증 체인 설계·운영

로또아이는 현재까지 1년 이상 해외 유사 사례를 확인하지 못한 점을 바탕으로, 위 두 가지 공개 검증 설계·운영 방식을 세계 최초 수준의 사례로 판단하고 사용하고 있습니다.

---

## 무엇을 기록하나요?

로또아이는 생성번호를 내부 시스템에만 보관하지 않고, 추첨 전에 외부 공개 문서인 Google 문서에 기록합니다.

회차별 Google 문서에는 생성번호 기록이 남고, 해당 문서는 고유한 URL을 가집니다.

Google 문서에서는 다음 내용을 확인할 수 있습니다.

- 실제 생성번호 기록
- 문서 생성 시점
- 데이터 저장 시점
- 권한 변경 이력
- 버전 기록
- 추첨 이후 수정 여부

이 저장소는 Google 문서 안의 생성번호 데이터를 직접 저장하는 공간이 아닙니다.  
본 저장소의 핵심 역할은 **각 회차의 Google 문서 URL을 추첨 전에 GitHub에 먼저 기록하는 것**입니다.

---

## 이 저장소의 역할

이 저장소는 로또아이 공개 검증 체인에서 **외부 기준 로그** 역할을 합니다.

Google 문서에는 실제 생성번호 기록이 남습니다.  
GitHub에는 해당 Google 문서 URL이 추첨 전에 먼저 기록됩니다.

따라서 누구나 추첨 이후 공개된 Google 문서 URL이 사후에 임의로 바뀐 것이 아닌지 GitHub 커밋 이력을 통해 확인할 수 있습니다.

즉, 이 저장소의 핵심 질문은 다음과 같습니다.

> **“이 Google 문서 URL이 추첨 전에 이미 외부 기록으로 남아 있었는가?”**

본 저장소는 이 질문에 대한 외부 기준점을 제공하기 위해 운영됩니다.

---

## 무엇을 검증할 수 있나요?

누구나 본 저장소의 GitHub 기록과 회차별 Google 문서를 대조하여 다음 내용을 확인할 수 있습니다.

1. **URL의 사전 고정 여부**  
   GitHub에 기록된 Google 문서 URL이 추첨 전에 존재했는지 확인할 수 있습니다.

2. **생성번호 기록의 존재 여부**  
   Google 문서에 생성번호 기록이 남아 있는지 확인할 수 있습니다.

3. **추첨 전 기록 기준**  
   Google 문서의 버전 기록을 통해 생성번호 데이터가 추첨 전 기준으로 존재했는지 검토할 수 있습니다.

4. **사후 변경 여부**  
   추첨 이후 Google 문서 또는 GitHub 기록에 변경이 발생했는지, 변경이 있었다면 그 시점과 내용을 확인할 수 있습니다.

로또아이는 사후 수정이 불가능하다고 주장하지 않습니다.  
대신 사후 수정 여부를 외부 기록으로 확인할 수 있는 검증 환경을 제공하는 것을 목표로 합니다.

---

## 공개 검증 체인 구조

로또아이의 공개 검증 체인은 다음 기준으로 구성됩니다.

```text
[Google 문서]
└ 실제 생성번호 기록 저장
└ 문서 생성 시점, 저장 시점, 버전 기록 확인 가능
↓
[GitHub 로그 저장소]
└ 회차별 Google 문서 URL을 추첨 전에 먼저 기록
└ 커밋 이력을 통해 URL의 사전 고정 여부 확인 가능
↓
[사후 검증]
└ 누구나 Google 문서와 GitHub 기록을 대조
└ 추첨 전 기록 존재 여부와 사후 변경 여부 확인
```

이 구조의 핵심은 단순히 외부에 기록을 남기는 것이 아닙니다.

실제 생성번호 기록이 담긴 Google 문서와,  
그 Google 문서 URL이 추첨 전에 고정되었다는 GitHub 기록을 함께 대조할 수 있도록 만드는 것입니다.

---

## 공개 검증 백서

로또아이 서비스 전체의 공개 검증 원칙, 운영 기준, 상세 검증 방법은 아래 백서에서 확인할 수 있습니다.

- [**로또아이 결과 공개 검증 백서 (Korean)**](./WHITEPAPER.md)
- [**LOTTOi Public Verification Whitepaper (English)**](./WHITEPAPER.en.md)

---

## 문서의 범위와 한계

본 저장소는 로또아이 공개 검증 체인의 외부 기준 로그를 제공하기 위한 저장소입니다.

본 저장소와 백서는 다음을 보장하지 않습니다.

- 당첨 확률
- 예측 성능
- 수익
- 특정 결과
- 투자 또는 구매 판단

본 저장소의 목적은 생성번호가 추첨 전에 외부 기록으로 남았는지, 그리고 사후 변경 여부를 누구나 확인할 수 있는 기준을 제공하는 것입니다.

---

## 🌐 Public Verification Overview (EN)

This repository is an external reference log repository within the **[LOTTOi](https://www.lottoi.kr)** public verification chain.

LOTTOi has applied a Google-based external public verification method since February 8, 2025.  
Since January 29, 2026, LOTTOi has operated a public verification chain that records each round’s Google document URL on GitHub before the draw.

The expression **“world-first-level external public verification and public verification chain”** used in this repository does not refer to lottery services as a whole.  
It refers to the design and operation of:

1. a Google-based external public verification method, and
2. a Google·GitHub-linked public verification chain.

Based on the fact that LOTTOi has not identified a similar overseas case for more than one year, LOTTOi uses this expression based on its judgment that the two verification design and operation methods above represent a world-first-level case.

In this structure, the actual generated number records are stored in Google documents.  
This GitHub repository records the corresponding Google document URLs before the draw.

This allows anyone to compare the GitHub commit history with the Google document records and check whether the disclosed verification URL was changed after the draw.

This repository does not guarantee winning probability, prediction performance, profit, or results.  
Its purpose is to provide an external reference point for verifying whether generated number records existed before the draw and whether any post-draw changes occurred.

For full technical details, please refer to the whitepapers linked above.
