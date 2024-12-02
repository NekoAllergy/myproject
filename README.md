# 첫 프로젝트(미배포)

개발기간 <br/>
1차 24.07 ~ 24.11 (4.5개월) <br/>
2차 24.12 ~ <br/>

개발 인원 1명

프로젝트 진행도(24년 12월 기준) <br/>
리소스 서버  <br/>
등록, 조회, 수정, 삭제 (80%)

UI <br/>
등록, 조회 페이지 (40%)


개발환경 <br/>
Vue3(Composition API) Nuxt3(SEO) <br/>
Spring Boot 3.3.4 <br/>
JPA(Hibernate-구현체, Criteria-동적쿼리) <br/>

하이브리드 웹앱 <br/>

서버 아키텍쳐 <br/>
모놀로식 Layered 하이브리드 아키텍처

1. 서버 코드를 물리적으로 분리하지않고 통으로 개발함 > 모놀로식
2. 물리적으로 분리하여 개발 > MSA(MicroService Architecture) <br/>

프로젝트 단위에 따라 모놀로식과 MSA 중 선택함 <br/>

Controller Service Repository Config Entity Dto 등 계층으로 구분한 Layered 아키텍쳐 <br/>
DDD(Domain Design Driven) > 폴더를 도메인(업무) 기준으로 나눔 <br/>
admin/website <br/>
member/website <br/>
ghost/website <br/>
 <br/>
레이어드 아키텍쳐와 DDD를 섞은 하이브리드 아키텍쳐 <br/>

<pre>
SIWA_Project
├── .idea
├── .mvn
├── .vscode
├── rawdotweb
├── src
│   └── main
│       └── java
│           └── com.main.web.siwa
│               ├── config
│               ├── controller
│               │   ├── admin.category
│               │   ├── auth
│               │   ├── ghost
│               │   ├── member
│               │   │   ├── comment
│               │   │   └── website
│               │   └── websiteImage
│               ├── dto
│               │   ├── admin.category
│               │   ├── auth
│               │   ├── ghost.website
│               │   ├── member
│               │   │   ├── comment
│               │   │   └── website
│               │   └── websiteImage
│               ├── entity
│               ├── error
│               ├── filter
│               ├── repository
│               │   ├── website
│               │   ├── member
│               │   └── comment
│               ├── service
│               │   ├── admin.category
│               │   ├── auth
│               │   ├── ghost.website
│               │   ├── member
│               │   │   ├── comment
│               │   │   └── website
│               │   └── websiteImage
│               └── utility

</pre>

배포 환경(예정)<br/>
우분투<br/>
ssh <br/>
Nginx<br/>


https://github.com/Amadeus-P/release_rawdotweb_resource_server <br/>


https://github.com/Amadeus-P/release_rowdotweb_client
