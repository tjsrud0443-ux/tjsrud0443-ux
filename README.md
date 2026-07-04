# 🧭 정선경 Portfolio

> 문제를 작게 나누고, 데이터 흐름을 끝까지 추적하며  
> 사용자에게 필요한 기능을 안정적으로 구현하는 Java/Spring 기반 풀스택 개발자 정선경입니다.

7년간 이커머스 운영 및 CS 관리 업무를 담당하며 사용자의 불편함이 어디서 발생하는지,  
데이터가 어떤 흐름으로 연결되어야 서비스가 안정적으로 동작하는지를 현장에서 체감했습니다.

개발자로 전환한 뒤에는 단순히 화면에 기능을 구현하는 것에서 그치지 않고,  
사용자의 요청이 프론트엔드, 백엔드, 데이터베이스, AI 서버까지 어떻게 이어지는지 끝까지 추적하며 개발하고 있습니다.

그룹웨어 프로젝트 **Orbit**에서는 조직도, 전자결재 문서함, 실시간 알림, 프로젝트 칸반보드,  
정형 DB 라우팅과 비정형 문서 검색을 결합한 **Hybrid RAG 기반 AI 챗봇**을 구현했습니다.

---

## 🛠 Tech Stack

### 🧩 Backend
- ☕ Java 17
- 🍃 Spring Boot
- 🌱 Spring MVC / Legacy
- 🗂 MyBatis
- 🔗 REST API
- 🔐 JWT
- 🔌 WebSocket / STOMP

### 🎨 Frontend
- ⚛️ React
- 🟨 JavaScript
- 🧱 HTML5
- 🎨 CSS3
- 🌬 Tailwind CSS
- 🐻 Zustand
- 📡 Axios
- 📊 Chart.js
- 🗺 Kakao Maps API

### 🗄 Database
- 🧡 Oracle DB

### 🤖 AI / Search
- ⚡ FastAPI
- 🧠 Spring AI
- 💬 Gemini / ChatClient
- 🔎 Qdrant
- 📌 BAAI/bge-m3
- 🧩 Hybrid RAG
- 🔍 Vector Similarity Search
- 🗃 Structured DB Routing

### ☁️ Infra / Deploy
- ☁️ AWS EC2
- ☁️ GCP Compute Engine
- 🗃 GCP Storage
- 🐳 Docker
- 🌐 Nginx
- 🔒 Certbot SSL
- 🔥 Firebase Hosting
- 🔄 GitHub Actions

### 🧰 Tools
- 🐙 Git / GitHub
- 💻 VSCode / Eclipse
- 🗄 Oracle SQL Developer
- 🎨 Figma
- 📐 Balsamiq
- 📝 Notion

---

## 📌 Projects

### 1. Orbit 🧭

> React + Spring Boot 기반 그룹웨어  
> 조직도, 전자결재 문서함, 프로젝트 관리/칸반보드, 실시간 알림, 회사 정보 등록/수정과 Hybrid RAG 기반 AI 챗봇을 포함한 협업 플랫폼

### 📖 프로젝트 개요

Orbit은 조직도, 전자결재 문서함, 프로젝트 관리, 일정, 근태, 실시간 알림, 관리자 기능,  
AI 챗봇을 포함한 사내 그룹웨어 시스템입니다.

사용자 질의 의도에 따라  
**정형 데이터는 Oracle DB 조회로 라우팅**하고,  
**비정형 데이터는 Qdrant 벡터 유사도 검색으로 라우팅**하는  
Hybrid RAG 기반 AI 챗봇을 설계하고 구현했습니다.

이를 통해 단순 문서 검색형 챗봇이 아니라,  
업무 데이터와 문서 검색을 함께 처리하는 사내 업무 비서 형태의 AI 기능을 구현했습니다.

### 🗓 개발 기간

2026.05 ~ 2026.06  
3인 팀 프로젝트

### ✨ 주요 기능

- 조직도 트리형 / 목록형 조회
- 부서 관리
- 전자결재 문서함
- 프로젝트 관리 및 칸반보드
- WebSocket 기반 실시간 알림
- 관리자 대시보드
- 회사 정보 등록 / 수정
- 사내 문서 / 회의록 기반 AI 챗봇
- AI 미답변 질문 관리
- 정형 DB 라우팅 + 비정형 문서 검색 기반 Hybrid RAG

### 🙋‍♀️ 담당 역할

- 조직도 트리형 / 목록형 조회 기능 구현
- 부서 및 사용자 정보 조회 흐름 구현
- 전자결재 문서함 기능 구현(나의 전자결재/결재할 문서함/참조 문서함/임시 문서함 4단 구조, 검색·상태별 조회·페이지네이션, 임시문서 자동삭제)
- 프로젝트 칸반보드 기능 구현
- WebSocket / STOMP 기반 실시간 알림 구현
- 회사 정보 등록 / 수정 기능 구현
- 관리자 대시보드 기능 구현
- AI 미답변 질문 관리 기능 구현
- 사내 문서 / 회의록 기반 AI 챗봇 기능 구현
- Orbit 서비스 전반의 Oracle DB 테이블 설계 및 관계 설정
- ERD 설계 및 주요 도메인 간 데이터 흐름 정리
- 더미데이터 구성 및 테스트 데이터 관리
- AI 챗봇 조회용 `V_AI_` View 설계 및 정형 데이터 조회 구조 구성
- AWS EC2 기반 Oracle DB 서버 구축 및 프로젝트 서버 연동 환경 구성
- GCP Compute Engine VM 내 Docker Compose 설정 및 디버깅 참여  
  - FastAPI, Qdrant 등 담당 AI 챗봇 기능 인프라 확인

### 🤖 RAG 챗봇 구현

- Gemini 기반 질의 라우팅으로 사용자 질문을 DB / DOC / UNKNOWN으로 분류
- 연차, 근태, 결재, 일정 등 정형 데이터 질문은 Spring AI Tool을 통해 Oracle DB 조회로 처리
- AI 챗봇 전용 `V_AI_` View를 구성하여 원본 테이블 직접 조회를 제한하고, 필요한 업무 데이터만 안전하게 제공
- DB 조회는 SELECT만 허용하고, SQL 키워드 블랙리스트·주석 차단·조회 건수 제한(ROWNUM)을 적용해 안전성 강화
- 사내 문서, 회의록, 규정 등 비정형 데이터 질문은 FastAPI와 Qdrant 기반 벡터 유사도 검색으로 처리
- 회의록 질문은 날짜, 월, 목록 조회 의도를 추가 분석해 관련 회의록 청크를 보정 검색
- BAAI/bge-m3 임베딩 모델을 활용해 문서와 회의록 청크를 벡터화
- Spring AI와 Gemini ChatClient를 연동해 검색 결과 기반 최종 답변 생성
- 비속어 필터를 적용해 부적절한 표현이 포함된 질문에 대한 답변 생성을 제한
- AI가 답변하지 못한 질문을 관리자가 확인할 수 있는 미답변 질문 관리 기능 구현

### 🛠 사용 기술

#### Core
- Java 17
- Spring Boot
- React
- MyBatis
- Oracle DB

#### API / Auth / Realtime
- REST API
- JWT
- WebSocket / STOMP
- Axios
- Zustand

#### AI / Search
- FastAPI
- Spring AI
- Gemini
- Qdrant
- BAAI/bge-m3
- Hybrid RAG
- Vector Similarity Search
- Structured DB Routing

#### Infra
- AWS EC2
- GCP Compute Engine
- GCP Storage
- Docker
- Nginx
- Firebase Hosting
- GitHub Actions

### 🌱 배운 점

- 프론트엔드, 백엔드, DB, AI 서버가 연결되는 전체 흐름을 경험했습니다.
- 단순 문서 검색형 RAG를 넘어, 질문 의도에 따라 정형 DB 조회와 비정형 문서 검색을 분기하는 구조를 구현했습니다.
- Spring Boot와 FastAPI, Qdrant를 연동하며 서로 다른 언어와 프레임워크 간 서비스 통신 구조를 경험했습니다.
- 실시간 알림, 권한 제어, 전자결재 문서함, 칸반보드처럼 실제 업무 시스템에서 필요한 기능 흐름을 이해했습니다.
- 배포 환경에서 DB와 서버가 연동되는 과정을 경험하며 운영 환경의 중요성을 배웠습니다.

---

### 2. 우리동네.ZIP 🏘

> Spring MVC / Legacy 기반 JSP 서버 사이드 렌더링 프로젝트  
> 공공 API 기반 지도 기능과 관리자 기능을 갖춘 지역 정보 커뮤니티 플랫폼

### 📖 프로젝트 개요

우리동네.ZIP은 지역 주민들이 동네 정보를 확인하고, 모임을 개설하며,  
지역 기반 안전 시설 정보를 확인할 수 있는 커뮤니티 서비스입니다.

Spring MVC / Legacy 기반의 서버 사이드 렌더링 구조로 구현했으며,  
공공데이터 기반 지도 기능, 모임 관리, 관리자 대시보드, 신고/블랙리스트 관리,  
Q&A 관리 기능을 중심으로 웹 서비스의 기본 흐름을 경험했습니다.

### 🗓 개발 기간

2026.03 ~ 2026.04  
5인 팀 프로젝트

### ✨ 주요 기능

- 공공데이터 기반 안심 지도
- 모임 리스트 조회 및 상태별 관리
- 카테고리별 모임 필터링
- 관리자 통계 대시보드
- 신고 / 블랙리스트 통합 관리
- 블랙리스트 사용자 로그인 제한
- Q&A 관리자 답변 CRUD
- 회원 정보 수정 및 탈퇴 처리

### 🙋‍♀️ 담당 역할

- 실무 PM으로 팀원 4명의 업무 분배, 회의 일정 조율, 개발 진척도 점검 및 팀원 간 의견 조율 수행
- 회원 정보 수정 및 탈퇴 처리 기능 구현
- 공공데이터 기반 안심 지도 기능 구현
- 모임 리스트 출력 및 상태별 관리 기능 구현
- 카테고리별 모임 필터링 및 상세 조건부 출력 기능 구현
- 관리자 통계 대시보드 구현
- 블랙리스트 / 신고 통합 관리 및 로그인 제한 기능 구현
- Q&A 기반 CS 관리 시스템의 관리자 답변 CRUD 기능 구현

### 🛠 사용 기술

#### Core
- Java
- Spring MVC / Legacy
- JSP
- Oracle DB

#### Feature
- JavaScript
- HTML
- CSS
- JSTL / EL
- Ajax
- Chart.js
- Kakao Maps API
- 공공데이터 API

#### Tools
- Git / GitHub
- Figma
- Balsamiq

#### Infra
- AWS EC2 배포 환경

### 🌱 배운 점

- Spring MVC 기반의 Controller, Service, DAO, JSP 흐름을 이해했습니다.
- 공공 API 데이터를 서비스 목적에 맞게 가공하고 지도 기능으로 연결하는 경험을 쌓았습니다.
- 모임, 지도, 관리자 기능처럼 여러 도메인이 연결되는 구조를 구현하며 데이터 흐름을 파악했습니다.
- 관리자 대시보드와 신고/블랙리스트 기능을 구현하며 운영자 관점에서 필요한 관리 흐름을 고민했습니다.
- 실무 PM 역할을 맡으며 일정 조율, 기능 분담, 진척도 관리, 팀원 간 의견 조율의 중요성을 배웠습니다.

---

## 💡 Project Experience Summary

두 번의 팀 프로젝트를 통해 웹 서비스의 기본 구조부터  
실제 업무 시스템에 가까운 서비스 흐름까지 단계적으로 경험했습니다.

1차 프로젝트 **우리동네.ZIP**에서는 Spring MVC / JSP 기반으로  
공공데이터 기반 지도 기능, 모임 리스트 및 상태 관리, 관리자 대시보드,  
신고/블랙리스트 관리, Q&A 관리자 답변 기능을 구현하며  
전통적인 서버 사이드 렌더링 구조와 MVC 흐름을 익혔습니다.

또한 실무 PM 역할을 맡아 팀원 4명의 업무 분배, 회의 일정 조율,  
개발 진척도 점검과 팀원 간 의견 조율을 수행하며  
기능 구현뿐 아니라 팀 프로젝트 운영 흐름도 함께 경험했습니다.

2차 프로젝트 **Orbit**에서는 React + Spring Boot 기반 그룹웨어 시스템을 구현하며  
조직도, 전자결재 문서함, 실시간 알림, 프로젝트 칸반보드, AI 챗봇 등  
실제 업무 흐름과 연결된 기능을 개발했습니다.

특히 Orbit 프로젝트에서는 전체 ERD 설계와 Oracle DB 테이블·데이터 관리를 주도하고,  
도메인별 더미데이터와 AI 챗봇 조회용 View를 구성하며  
기능 구현에 필요한 데이터 구조와 흐름을 직접 관리했습니다.

또한 FastAPI, Qdrant, Spring AI, Gemini를 연동하여  
정형 DB 조회와 비정형 문서 검색을 함께 처리하는  
Hybrid RAG 기반 AI 챗봇을 구현했습니다.

AWS EC2 환경에서는 Oracle DB 서버를 구축하고 프로젝트 서버와 연동하며,  
로컬 개발 환경을 넘어 실제 배포 환경에서 DB가 연결되고 동작하는 흐름까지 경험했습니다.

7년간의 이커머스 운영 및 CS 경험은  
기능을 구현할 때 “사용자가 실제로 어떤 상황에서 이 기능을 쓰게 될지”를 먼저 고민하는 습관으로 이어지고 있습니다.

---

## 🎓 Education

### 한국정보교육원
**현업에서 바로 통하는 자바 풀스택 & 생성형 AI 서비스 개발 기업 프로젝트 완성**

- 기간: 2025.12 ~ 2026.07
- Java, Spring, Oracle DB, JavaScript, React 기반 웹 개발 학습
- 팀 프로젝트를 통해 지역 커뮤니티 플랫폼과 기업형 그룹웨어 시스템 구현
- RAG 기반 AI 챗봇, 실시간 알림, 전자결재 문서함, 조직도, 프로젝트 칸반보드 등 업무 시스템 기능 구현 경험

---

## 📫 Contact

- ✉️ Email: tjsrud0443@gmail.com
- 🐙 GitHub: [github.com/tjsrud0443-ux](https://github.com/tjsrud0443-ux)
- 📝 Notion: [Notion Portfolio](https://complex-chord-dba.notion.site/Portfolio-1ebc59b1c172828a8ef7812704f611fa?source=copy_link)
- 🌐 Portfolio: [SunKyung.dev](https://sunkyungdev.netlify.app/)
