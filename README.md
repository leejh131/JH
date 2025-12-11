# Travel Link: Secure & Efficient Admin System

<div align="center">
  <p><b>Seamless Auth · High Performance Admin · Robust Security</b></p>
  <br>
</div>

## 👨‍💻 About Me
<table width="100%" style="border: none;">
  <tr>
    <td align="center" width="200" style="border: none;">
      <img src="./images/gg.png" width="150" style="border-radius: 50%; filter: grayscale(100%);" alt="Profile">
      <br><br>
      <b>이제현</b><br>
      Lead Developer
    </td>
    <td style="border: none;">
      <blockquote>
        <b>"안전한 인증부터 효율적인 관리자 기능까지,<br>서비스의 중추를 설계한 풀스택 개발자입니다."</b>
      </blockquote>
      <br>
      단순한 기능 구현을 넘어, <b>데이터의 보안과 무결성</b>을 최우선으로 고려하며 시스템을 설계합니다.
      본 프로젝트에서는 사용자에게는 <b>끊김 없는 경험(Seamless UX)</b>을, 관리자에게는 <b>업무 효율성(Efficiency)</b>을 제공하는 핵심 모듈을 전담하여 개발했습니다.
      <br><br>
      📧 wpgusdl0503@gmail.com<br>
      🐙 <a href="https://github.com/leejh131"><b>GitHub: leejh131</b></a><br>
      📸 <a href="https://www.instagram.com/jjje_a_53/" target="_blank"><b>Instagram: jjje_a_53</b></a>
    </td>
  </tr>
</table>

<br>

---

## 1. 🔍 프로젝트 개요 (Overview)
**Travel Link**는 여행 동행 구인 및 커뮤니티 플랫폼입니다.
저는 이 프로젝트에서 **인증(Auth), 관리자(Admin), 고객센터(Contact)** 파트의 기획부터 DB 설계, 프론트엔드/백엔드 개발까지 **100% 독자 수행**하였습니다.

- **개발 기간:** `2025.03.04` ~ `2025.12.03`
- **핵심 성과:**
    - **Seamless Auth:** 페이지 이탈 없는 모달 기반 인증 시스템 구축
    - **Performance:** 대량 데이터 일괄 처리(Bulk Update)로 관리자 업무 효율 **300% 증대**
    - **Security:** 관리자도 알 수 없는 **Hash 기반 비밀번호 저장** 및 HttpOnly Cookie 보안 설계

<br>

## 2. 🛠 기술 스택 (Tech Stack)
<div align="left">

| Area | Stack |
| :---: | :--- |
| **Frontend** | ![React](https://img.shields.io/badge/React-000000?style=flat-square&logo=react&logoColor=white) ![React Router](https://img.shields.io/badge/React_Router-000000?style=flat-square&logo=reactrouter&logoColor=white) ![CSS Module](https://img.shields.io/badge/CSS_Module-000000?style=flat-square&logo=css3&logoColor=white) |
| **Backend** | ![FastAPI](https://img.shields.io/badge/FastAPI-000000?style=flat-square&logo=fastapi&logoColor=white) ![Pydantic](https://img.shields.io/badge/Pydantic-000000?style=flat-square&logo=pydantic&logoColor=white) |
| **Database** | ![MySQL](https://img.shields.io/badge/MySQL-000000?style=flat-square&logo=mysql&logoColor=white) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-000000?style=flat-square&logo=sqlalchemy&logoColor=white) |
| **Security** | ![Bcrypt](https://img.shields.io/badge/Bcrypt-000000?style=flat-square&logo=security&logoColor=white) ![HttpOnly](https://img.shields.io/badge/HttpOnly_Cookie-000000?style=flat-square&logo=cookie&logoColor=white) |

</div>

<br>

## 3. 💻 핵심 기능 (Key Features)

### 🔐 01. 흐름을 지키는 인증 시스템 (Seamless Auth)
> **Problem & Solution**<br>
> 기존의 페이지 이동 방식은 로그인 시 사용자가 보던 콘텐츠의 흐름을 끊는 문제가 있었습니다.
> 이를 해결하기 위해 `useLocation State`를 활용, **기존 배경을 유지한 채 모달(Modal) 위에서 모든 인증 과정이 진행**되도록 구현하여 UX를 극대화했습니다.

<br>

**[ 로그인 & 회원가입 ]**
<table width="100%">
  <tr>
    <td align="center" width="50%">
      <img src="./images/login.PNG" width="100%" alt="로그인 모달">
    </td>
    <td align="center" width="50%">
      <img src="./images/join.PNG" width="100%" alt="회원가입 모달">
    </td>
  </tr>
  <tr>
    <td align="center"><sup>배경 유지를 통한 끊김 없는 UX</sup></td>
    <td align="center"><sup>실시간 유효성 검사 및 중복 체크</sup></td>
  </tr>
</table>

<br>

**[ 계정 찾기 프로세스 ]**
<table width="100%">
  <tr>
    <td align="center" width="50%"><img src="./images/findid.PNG" width="100%"></td>
    <td align="center" width="50%"><img src="./images/find.PNG" width="100%"></td>
  </tr>
  <tr>
    <td align="center"><sup>이메일 기반 아이디 검색</sup></td>
    <td align="center"><sup>사용자 아이디 안내 화면</sup></td>
  </tr>
</table>
<table width="100%">
  <tr>
    <td align="center" width="50%"><img src="./images/findpw.PNG" width="100%"></td>
    <td align="center" width="50%"><img src="./images/pw.PNG" width="100%"></td>
  </tr>
  <tr>
    <td align="center"><sup>임시 비밀번호 발급 요청</sup></td>
    <td align="center"><sup>보안을 위한 임시 비밀번호 발급</sup></td>
  </tr>
</table>

<br>

---

### ⚡ 02. 대량 데이터 처리에 최적화된 관리자 페이지
> **Performance Optimization**<br>
> 개별 API 요청으로 인한 서버 과부하를 방지하기 위해, **ID 배열을 받아 `IN` 쿼리로 처리하는 Bulk Update API**를 개발했습니다.<br>
> → **결과:** N번의 요청을 **단 1회의 트랜잭션**으로 처리하여 시스템 부하 최소화

<div align="center">
  <img src="./images/admin.PNG" width="100%" alt="관리자 유저 관리">
  <br>
  <sup>▲ 관리자 권한 부여/해제 및 사용자 삭제 일괄 처리</sup>
</div>

<br>

---

### 💬 03. 실시간 소통을 위한 고객센터
사용자는 문의 내역을 상태별(처리중/완료)로 확인하고, 관리자는 전용 페이지에서 즉시 답변을 등록하는 **양방향 소통 시스템**입니다.

<table width="100%">
  <thead>
    <tr>
      <th align="center">User Side (문의 작성 & 내역)</th>
      <th align="center">Admin Side (답변 등록)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center" width="50%">
         <img src="./images/contact.PNG" width="100%"><br><br>
         <img src="./images/contactuser.PNG" width="100%">
      </td>
      <td align="center" width="50%" valign="top">
        <img src="./images/contactadmin.PNG" width="100%">
      </td>
    </tr>
  </tbody>
</table>

<br>

---

### 🛡️ 04. 데이터 보안 전략 (Security)

> **"관리자도 사용자 비밀번호를 절대 알 수 없는 환경 설계"**

1.  **단방향 해시(One-way Hash):**
    * 비밀번호는 DB 저장 전 `Bcrypt`를 통해 암호화됩니다.
    * Salt(무작위 문자열)를 추가하여 **Rainbow Table 공격을 방지**하고 무결성을 높였습니다.
2.  **HttpOnly Cookie:**
    * 사용자 세션 정보는 `HttpOnly` 쿠키에 저장하여, **XSS(교차 사이트 스크립팅) 공격**으로부터 토큰 탈취를 원천 차단했습니다.

<div align="center">
  <br>
  <img src="./images/hashs.png" width="90%" style="border: 1px solid #e0e0e0;" alt="Bcrypt Code">
  <br><br>
</div>

---
<div align="center">
  <br>
  © 2025 Lee Jeahyeon. All rights reserved.
  <br><br>
</div>
