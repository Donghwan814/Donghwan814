<h2 align="center">김동환 · Backend Developer</h2>

<p align="center">
  <b>끊기고 몰려도 데이터가 맞는 서버를 만듭니다.</b><br>
  Java 21 · Spring Boot · JPA · MySQL / PostgreSQL · Docker · AWS
</p>

<p align="center">
  <a href="https://donghwan814.github.io/"><img src="https://img.shields.io/badge/Portfolio-donghwan814.github.io-3D5AFE?style=flat-square" /></a>
  <a href="mailto:kdh969512@gmail.com"><img src="https://img.shields.io/badge/Email-kdh969512@gmail.com-555?style=flat-square&logo=gmail&logoColor=white" /></a>
  <img src="https://img.shields.io/badge/신한대_소프트웨어융합학과-2027.02_졸업예정-555?style=flat-square" />
</p>

---

### 🏆 수상

| 시기 | 내용 | 내 역할 |
|---|---|---|
| 2026.11 | **2026 멋쟁이사자처럼 1호선톤 최우수상** (8개 대학 연합) | FITMATE 실시간 WebSocket 서버 |
| 2026.08 | 멋사 중앙 해커톤 SJF 트랙 **82팀 중 상위 15팀** | MTM 백엔드 |
| 2025.10 | SW중심대학 SUMTECH 해커톤 **장려상** | Re:Form 팀장 · 백엔드 |

---

### 🔧 대표 프로젝트

| 프로젝트 | 무엇을 했나 | 근거 |
|---|---|---|
| **[FITMATE](https://github.com/20thTeam/fitmate-be)** <br> 친구와 같은 방에서 하는 AI 홈트 · 최우수상 | 운동방 WebSocket 중계 계층 전담. 끊김 30초 자리 유지·재접속 복원, 메시지 크기·빈도 상한, 사칭 차단 | 15Hz 동작 정보 **20명 동시 p95 29ms · 손실 0%** 실측 · 테스트 **245건** |
| **[비콘 출결 플랫폼](https://github.com/Dev-MAMOKEY/Beacon-Backend)** <br> 산학연계 · 실운영 | 백엔드 전담. BLE 근접 + 인증번호 이중 조건, 감지 임계값 설정화, (회원, 세션) 유니크로 중복 출석 차단 | 운영 중 **전 API 500 장애**(OSIV + SSE로 커넥션 풀 고갈) 원인 규명·재발 감지 |
| **[한국어 발음 교정](https://github.com/Shinhan-KoreanLanguage/backend)** <br> 졸업작품 | 서버 단독. JWT·소셜 로그인, 외부 AI 서버 격리(연결 5s / 응답 60s), N+1 일괄 조회 | 커밋 **243건 중 208건** · API 36개 · 에러코드 46종 |
| **[진상 멈춰](https://github.com/jinsang-stop/jinsang-stop-backend)** <br> 로컬 LLM 민원 응대 훈련 | 1인 백엔드. 음성·LLM 서비스 오케스트레이션, 진행 세션 유니크 제약, Flyway, LLM 출력 검사·재시도 | 테스트 **124건** · ADR 기반 설계 |
| **[MTM](https://github.com/Dev-MAMOKEY/MTM-Backend)** <br> AI 가상 착용 | (사진, 제품) 조합 결과 재사용, 생성 공급자 인터페이스로 OpenAI→Gemini 교체 | 응답 **9.595초 → 0.033초** |

---

### 🧯 직접 해결한 장애

- **커넥션 풀 고갈** — SSE 배포 직후 전 API 500. OSIV가 최대 30분짜리 SSE 요청의 커넥션을 붙잡아 풀 10개가 고갈. `open-in-view` 비활성화 + 누수 감지 설정, 배포 이미지 누락을 막으려 컨테이너 환경변수에 이중 명시.
- **운영에서만 9시간 어긋난 시각** — 컨테이너 UTC 기동이 원인. Dockerfile·애플리케이션·환경변수 3중 고정, 기존 데이터는 마이그레이션으로 정정.
- **S3 고아 파일** — `ON DELETE CASCADE`로 행이 지워지면 저장소 키를 잃음. 키를 먼저 모으고 자식부터 삭제, 파일 삭제는 커밋 이후로 이동.

---

### 🛠 Stack

`Java 21` `Spring Boot` `Spring Security` `Spring Data JPA` `Spring WebSocket` `JWT · OAuth2`
`MySQL` `PostgreSQL` `H2` `Flyway`
`Docker` `Docker Compose` `AWS EC2 · RDS · S3` `Nginx` `GitHub Actions`
`JUnit 5` `Swagger(springdoc)` `Postman` · 자격: `SQLD` `TOPCIT Level 3`

### 📐 일하는 방식

- 이슈 하나 = 브랜치 하나 = PR 하나. PR마다 변경 사항 · 범위 · 테스트 결과 · Postman 예시를 남깁니다.
- 구현 전에 용어집(`CONTEXT.md`)과 ADR로 결정 근거를 먼저 적습니다.
- 숫자는 직접 측정한 값만, 측정 조건과 함께 씁니다.
