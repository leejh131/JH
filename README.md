# ✈️ Travel Link: Secure & Efficient Admin System

> **안전한 인증(로그인)부터 효율적인 관리자 기능까지, 서비스의 중추를 설계한 풀스택 개발자 이제현입니다.**

![Login Screen](./images/login.PNG)

<br>

## 1. 프로젝트 개요 (Project Overview)
단순한 데이터 조회를 넘어, 사용자 경험(UX)과 관리자 업무 효율을 동시에 극대화하는 여행 커뮤니티 관리 시스템을 구축했습니다.
**본 프로젝트에서 인증(Auth), 관리자(Admin), 고객센터(Contact) 모듈의 기획부터 배포까지 전담하였습니다.**

* **개발 기간:** 2025.XX ~ 2025.XX
* **담당 역할:** Lead Developer (Full Stack)
* **주요 기여:**
    * 페이지 이탈 없는 **Modal Routing** 인증 시스템 구현
    * **Bulk Update**를 통한 관리자 데이터 처리 성능 최적화
    * **1:1 문의 시스템** 및 관리자 답변 기능 구현

<br>

## 2. 기술 스택 (Tech Stack)
| Area | Stack |
|:---:|:---|
| **Frontend** | React, React Router, CSS Module |
| **Backend** | FastAPI, Pydantic |
| **Database** | MySQL, SQLAlchemy |
| **Security** | Bcrypt, HttpOnly Cookie |

<br>

## 3. 핵심 기능 (Key Features)

### 🔐 1. 사용자 경험을 고려한 인증 시스템 (Authentication)
**"흐름이 끊기지 않는 로그인/회원가입 경험"**
기존 페이지의 배경을 유지한 채 모달(Modal) 위에서 모든 인증 절차가 이루어지도록 `useLocation State`를 활용해 라우팅을 처리했습니다.

| 회원가입 (Sign Up) |
| :---: |
| <img src="./images/join.PNG" width="100%"> |
| **이메일 중복 확인 및 유효성 검사 적용** |

<br>

**[계정 찾기 기능]**
사용자가 계정 정보를 잊었을 때를 대비해 아이디/비밀번호 찾기 기능을 별도 모달로 구현했습니다.

| 아이디 찾기 | 비밀번호 찾기 |
| :---: | :---: |
| <img src="./images/findid.PNG" width="100%"> | <img src="./images/findpw.PNG" width="100%"> |

<br>

---

### ⚡ 2. 효율적인 관리자 시스템 (Admin System)
**"수십 명의 권한을 단 한 번의 클릭으로 수정"**
관리자 페이지에서 다수의 회원 권한을 수정할 때, 개별 API 요청(N번) 대신 ID 배열을 받아 **단 1회의 트랜잭션(`IN` 쿼리)**으로 처리하여 서버 부하를 최소화했습니다.

![Admin User Management](./images/admin.PNG)
* **주요 기능:** 회원 목록 조회, 검색, 관리자 권한 부여/해제 일괄 처리

<br>

---

### 💬 3. 1:1 문의 및 고객센터 (Customer Support)
**"사용자와 관리자를 잇는 소통 채널"**
사용자는 문의글을 남기고 처리 상태를 확인할 수 있으며, 관리자는 전용 페이지에서 답변을 등록할 수 있습니다.

**[사용자 화면: 문의 작성 및 내역 확인]**
| 문의 작성 (Write) | 문의 내역 (History) |
| :---: | :---: |
| <img src="./images/contact.PNG" width="100%"> | <img src="./images/contactuser.PNG" width="100%"> |

<br>

**[관리자 화면: 답변 관리]**
관리자는 접수된 문의글을 상태별(미답변/완료)로 확인하고 답글을 작성합니다.

![Admin Contact Management](./images/contactadmin.PNG)

<br>

---
**Contact:** wpgusdl0503@gmail.com
