# 🛒 LKS_Dashimarket — My Contribution Portfolio

> 더 나은 시스템을 향해 도전하며, 끊임없이 성장을 추구하는 개발자 이규식입니다.

---

## 🔎 Project Overview

**Dashimarket(다시마켓)** 은  
중고 거래, 친환경 굿즈 판매, 커뮤니티 기능을 통합한 마켓플레이스 플랫폼입니다.

단순 거래 종료형 서비스가 아닌,  
거래 이후에도 사용자가 참여하고 소통할 수 있는 구조를 목표로 기획되었습니다.

본 저장소는 팀 프로젝트에서 제가 직접 설계·구현한 영역과 문제 해결 과정을 정리한
개인 포트폴리오 문서 저장소입니다.

- 🧑‍💻 Role: Team Leader / FullStack Developer  
- 🗓 Period: 2025.09.15 ~ 2025.10.20 (약 1개월)  
- 👥 Team: 6 members  
- 🔗 Team Repository: https://github.com/Team-Nuguri/dashimarket  

---

## 🧑‍💻 My Role & Responsibility

### 👑 주요 기여

#### 🛍 상품 및 거래 시스템 구현
- 중고 상품 및 굿즈 상품 CRUD 기능 구현
- 다중 이미지 업로드 및 썸네일 처리 로직 구현
- Ajax 기반 비동기 수량 변경 및 화면 즉시 반영
- 장바구니 기능 개발 (상품 추가·수량 변경·결제 연동)
- 거래 상태 관리 및 주문 내역 관리 기능 구현
- 상품 QnA 등록·조회 및 비밀글 기능 구현
- 거래 완료 후 리뷰 작성 및 조회 기능 구현

#### 💳 외부 API 연동 (결제 / 소셜 로그인)
- PortOne API 기반 상품 결제 기능 구현
- 주문 금액과 실제 결제 금액 비교 검증 로직 설계
- Kakao 소셜 로그인 연동
- Spring Security OAuth2 기반 사용자 정보 가공 및 인증 처리

#### 🗄 데이터 설계 및 구조 정의
- Figma 기반 서비스 와이어프레임 설계
- ERD 설계를 통한 회원·상품·주문·장바구니 데이터 모델 정의
- 기능 흐름 기반 API 설계 및 페이지 구조 구성

---

## 🧪 문제 해결 경험

### 💥 Case: 외부 API 연동 과정에서의 요청–응답 구조 이해 부족

#### 🧩 Problem
외부 API(소셜 로그인, 결제)를 처음 연동하면서  
요청 방식, 파라미터 구조, 응답 데이터 흐름에 대한 이해 부족으로  
반복적인 오류가 발생했습니다.

#### 🔎 Cause
- 요청–응답 흐름에 대한 구조적 이해 부족  
- 필수 파라미터 및 응답 데이터 처리 로직 미정의  
- API 연동을 기능 단위로 접근하며 전체 서비스 흐름과 연결되지 못함  

#### 🛠 Solution
- 공식 문서를 기반으로 요청 URL, 방식, 파라미터, 응답 구조를 정리  
- 요청–응답 흐름을 문서화하고 단계별로 구현  
- Spring Security OAuth2 적용 후 사용자 정보 가공 로직 직접 구현  
- 결제 성공·실패·취소 시 DB 정합성을 유지하도록 로직 보완  
  - 결제 실패 시 주문 데이터 삭제  
  - 주문 금액과 실제 결제 금액 비교 검증 로직 추가  

#### ✅ Result
- 소셜 로그인 및 결제 기능을 안정적으로 서비스에 통합  
- 외부 시스템 연동 시 전체 흐름 이해의 중요성을 체득  

---

## 📸 주요 기능 화면

- 상품 등록 및 관리 화면
<img width="500" height="500" alt="{DE9BAC48-DD3B-45AC-A9EF-BEAA235D9CBD}" src="https://github.com/user-attachments/assets/5f18f871-e355-408c-809a-8c6687ab3e18" />
<br><br>

- 장바구니 및 결제 화면
<div style="display: flex; gap: 10px;">
  <img src="https://github.com/user-attachments/assets/a43d8609-860d-4422-9c71-aaa2dc6aef1f" width="500"/>
  <img src="https://github.com/user-attachments/assets/403afb55-cb68-4835-876b-dc6a66edb835" width="500" height="300"/>
</div>
<br><br>

- 소셜 로그인 연동 화면  
 <img width="377" height="398" alt="{D155BE0B-3B70-4B0A-A203-97447FAC41D4}" src="https://github.com/user-attachments/assets/1459bb09-58e9-4de9-94c9-f3ccfba08340" />


---

## 🚀 What I Learned

- 구현 전에 흐름을 구조화하는 습관이 개발 속도와 정확도를 높인다는 것을 경험  
- 외부 API 문서를 기반으로 전체 요청–응답 사이클을 정리하는 방법을 익힘  
- 데이터 정합성과 상태 관리 관점에서 기능을 바라보는 사고방식으로 전환  

---

## 📬 Contact

- Email: holysik.dev@gmail.com
