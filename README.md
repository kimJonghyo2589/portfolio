# 🖥️ CodeMoa
> 개발자들을 위한 커뮤니티 + 정보 공유 + 팀/채용 매칭 플랫폼

---

## 📌 프로젝트 개요
- **프로젝트명**: CodeMoa  
- **개발 목적**: 개발자, 예비 개발자, 개발 학습자를 위한 정보 공유·소통·팀/채용 매칭 플랫폼 구축  
- **개발 기간**: 2025.07 ~ 2025.08  
- **팀 규모**: 5명 (본인 포함)  
- **주요 기술 스택**:  
  - Backend: Spring Boot, Spring Security, JPA  
  - Frontend: Thymeleaf, HTML5, CSS3, JavaScript  
  - DB: MySQL  
- **타깃 사용자**: 개발자, 예비 개발자, 개발 학습자

---

## 🎯 팀 전체 목표
CodeMoa는 개발자 생태계에서 필요한 **정보 공유**, **협업 기회 제공**, **취업 연결**을 한곳에서 해결하는 것을 목표로 했습니다.  
주요 기능은 다음과 같습니다:
1. **커뮤니티**: 개발 관련 게시판, 댓글, 좋아요 기능
2. **채용 정보 제공**: Open API 기반 채용 공고 수집·검색
3. **팀 매칭**: 프로젝트 구인/구직 게시판
4. **회원 인증 및 권한 관리**: Spring Security 기반 로그인/회원가입

---

## 🛠️ 담당 역할 (My Contribution)
> 본인은 프로젝트에서 **채용 공고 수집 및 검색 기능** 구현을 주로 담당했습니다.

- 워크넷(고용24) Open API 연동 및 XML 데이터 파싱  
- DTO 변환 및 채용 공고 DB 저장 로직 개발  
- 채용 공고 목록 조회, 검색, 페이징 기능 구현  
- Thymeleaf 기반 채용 공고 목록 및 상세보기 페이지 구현  
- XML 파싱 중 특수문자 인코딩 문제 해결

---

## 🗂️ 시스템 아키텍처
```plaintext
[사용자 브라우저]
      │ (HTTP 요청)
      ▼
[Spring Boot Controller]  ← (Thymeleaf View Rendering)
      │
      ▼
[Service Layer] ────> [OpenAPI 호출 (WorkNet)]
      │                     │
      ▼                     ▼
[Repository / JPA]    (XML 데이터 수신 및 파싱)
      │
      ▼
[MySQL DB]
```

## 🗂️ 시스템 아키텍처
# 1. 레포지토리 클론
git clone https://github.com/orionrich1/codemoa.git

# 2. 프로젝트 폴더로 이동
cd codemoa

# 3. 실행
./gradlew bootRun

