# lottoi-googleurl-verification-log

이 저장소는 **로또아이(LOTTOi)** 서비스의  
**결과 공개 검증 구조**를 구성하는  
**외부 기준 로그(verification log)** 저장소입니다.

---

## 무엇을 기록하나요?

로또아이는 각 회차마다 회원이 생성한 번호를  
**추첨 이전 시점**에 **외부 문서(Google 공개 문서)** 형태로 기록합니다.

이 Google 문서는 회차별로 **고유한 URL**을 가지며,  
다음 정보가 외부 시스템에 자동으로 남습니다.

- 문서가 **언제 처음 생성되었는지**
- 이후 **어떤 변경이 있었는지**
- 각 변경의 **시간 순서**

---

## 이 저장소의 역할은 무엇인가요?

이 저장소는 Google 문서 자체를 대신 검증하거나  
내용을 보증하는 공간이 아닙니다.

대신, 각 회차의 **Google 공개 문서 URL이  
추첨 이전에 이미 외부에 존재했는지**를  
회차별·시간 순서대로 기록·공개하기 위한  
**외부 기준 로그(anchor)** 역할을 합니다.

즉,  
> “이 URL이 언제부터 존재했는가?”  
를 외부에서 다시 한 번 확인할 수 있도록  
**시간 기준의 로그를 공개적으로 남기는 공간**입니다.

---

## 무엇을 검증할 수 있나요?

이 저장소의 로그와 Google 문서를 함께 확인하면,

- Google 문서의 **생성 시점**
- GitHub에 기록된 **URL 로그 시점**
- 문서의 **변경 이력**

을 서로 비교하여,

> 결과 기록이 **추첨 이후에 사후 조작되었는지 여부**를  
> 누구나 외부에서 직접 확인·검토할 수 있습니다.

이는 로또아이 서비스 전반에서 사용하는  
**공개 검증 구조의 일부**입니다.

---

## 공개 검증 기준에 대하여

본 저장소는 Google 공개 문서 URL의 존재 시점을  
외부에 고정하기 위한 시간 기준 로그(anchor) 역할을 합니다.

로또아이 서비스 전체의 공개 검증 원칙,  
운영 기준, 검증 방법에 대한 자세한 설명은  
아래 백서 문서를 참고해 주세요.

- [로또아이 결과 공개 검증 백서 (Korean)](./WHITEPAPER.md)
- [LOTTOi Public Verification Whitepaper (English)](./WHITEPAPER.en.md)

---

## Public Verification Whitepaper (EN)

This repository serves as an **external verification log**  
within LOTTOi’s public verification system.

It records when each Google public document URL  
first existed externally, allowing anyone to verify  
whether records were created **before the lottery draw**  
and whether any changes occurred afterward.

For the full verification structure and operational principles,  
please refer to the whitepaper documents linked above.
