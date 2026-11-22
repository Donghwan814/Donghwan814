<p align="center">
  <img 
    src="https://capsule-render.vercel.app/api?type=waving&color=0:667eea,50:7C3AED,100:764ba2&height=260&section=header&text=Donghwan%20%7C%20Backend%20Developer&fontSize=42&fontColor=ffffff&animation=twinkling&fontAlignY=38&desc=Java%20%C2%B7%20Spring%20Boot%20%C2%B7%20Real-time%20%C2%B7%20Data%20Consistency&descAlignY=60&descSize=18" 
  />
</p>

<h3 align="center">끊기고 몰려도 데이터가 맞는 서버를 만듭니다.</h3>

<p align="center">
  <a href="https://git.io/typing-svg">
    <img 
      src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=23&pause=1000&color=7C3AED&center=true&vCenter=true&width=850&lines=2026+LIKELION+Line-1+Hackathon+Grand+Prize;Real-time+WebSocket+Relay+%7C+p95+29ms+%40+20+users;Root-caused+a+Connection+Pool+Outage+in+Production;Every+Rule+Pinned+Down+by+Tests" 
      alt="Typing SVG" 
    />
  </a>
</p>

<p align="center">
  <a href="https://donghwan814.github.io/"><img src="https://img.shields.io/badge/Portfolio-donghwan814.github.io-7C3AED?style=for-the-badge&logo=githubpages&logoColor=white" /></a>
  <a href="mailto:kdh969512@gmail.com"><img src="https://img.shields.io/badge/kdh969512@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/1%ED%98%B8%EC%84%A0%ED%86%A4-%EC%B5%9C%EC%9A%B0%EC%88%98%EC%83%81-FFB000?style=for-the-badge&logo=trophy&logoColor=white" />
  <img src="https://img.shields.io/badge/Backend-Developer-7C3AED?style=for-the-badge&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/%EC%8B%A0%ED%95%9C%EB%8C%80_%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4%EC%9C%B5%ED%95%A9-2027.02_%EC%A1%B8%EC%97%85%EC%98%88%EC%A0%95-555555?style=for-the-badge" />
</p>

---

## 👋 About Me

```java
public class Donghwan {
    private String role       = "Backend Developer";
    private String mainStack  = "Java 21, Spring Boot, JPA, MySQL, PostgreSQL";
    private String focus      = "Real-time, Data Consistency, Incident Analysis";
    private String award      = "2026 LIKELION Line-1 Hackathon Grand Prize";
    private String habit      = "Measure -> Fix -> Pin it with tests";
}
```

---

## 🏆 Awards

| 시기 | 내용 | 내 역할 |
|:---:|---|---|
| 2026.11 | **2026 멋쟁이사자처럼 1호선톤 최우수상** (8개 대학 연합) | FITMATE 실시간 WebSocket 서버 |
| 2026.08 | 멋사 중앙 해커톤 SJF 트랙 **82팀 중 상위 15팀** | MTM 백엔드 |
| 2025.10 | SW중심대학 SUMTECH 해커톤 **장려상** | Re:Form 팀장 · 백엔드 |

---

## 🚀 Featured Projects

| 프로젝트 | 핵심 구현 | 성과 |
|---|---|---|
| **[FITMATE](https://github.com/20thTeam/fitmate-be)** <br> 🏆 최우수상 | 운동방 WebSocket 중계, 끊김 30초 자리 유지·재접속 복원, 크기·빈도 상한, 사칭 차단 | **20명 동시 p95 29ms · 손실 0%** <br> 테스트 **245건** |
| **[비콘 출결 플랫폼](https://github.com/Dev-MAMOKEY/Beacon-Backend)** <br> 산학연계 · 실운영 | BLE + 인증번호 이중 출석, 임계값 설정화, 복합 유니크로 중복 출석 차단 | 운영 **전 API 500 장애** 원인 규명·해결 |
| **[한국어 발음 교정](https://github.com/Shinhan-KoreanLanguage/backend)** <br> 졸업작품 · 서버 단독 | JWT·소셜 로그인, 외부 AI 서버 격리, N+1 제거 | API **36개** · 커밋 **208건** |
| **[진상 멈춰](https://github.com/jinsang-stop/jinsang-stop-backend)** <br> 1인 백엔드 | 음성·LLM 서비스 오케스트레이션, Flyway, LLM 출력 검사·재시도 | 테스트 **124건** |
| **[MTM](https://github.com/Dev-MAMOKEY/MTM-Backend)** <br> 상위 15팀 | (사진, 제품) 결과 재사용, 생성 공급자 교체 구조 | **9.595초 → 0.033초** |

---

## 🧯 Troubleshooting

| 문제 | 원인 | 해결 |
|---|---|---|
| SSE 배포 직후 **전 API 500** | OSIV + 장시간 SSE가 커넥션 풀 10개 고갈 | `open-in-view` 비활성화, 누수 감지 설정, 환경변수 이중 명시 |
| 운영에서만 **시각 9시간 오차** | 컨테이너 UTC 기동 | 타임존 3중 고정, 기존 데이터 마이그레이션 정정 |
| 사진 삭제 후 **S3 고아 파일** | CASCADE로 저장소 키 유실 | 키 선수집, 파일 삭제를 커밋 이후로 이동 |

---

## ✨ Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white" />
  <img src="https://img.shields.io/badge/JPA-59666C?style=for-the-badge&logo=hibernate&logoColor=white" />
  <img src="https://img.shields.io/badge/WebSocket-010101?style=for-the-badge&logo=socketdotio&logoColor=white" />
  <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Flyway-CC0200?style=for-the-badge&logo=flyway&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/JUnit5-25A162?style=for-the-badge&logo=junit5&logoColor=white" />
  <img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black" />
  <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" />
  <img src="https://img.shields.io/badge/SQLD-Certified-003B57?style=for-the-badge" />
  <img src="https://img.shields.io/badge/TOPCIT-Level%203-003B57?style=for-the-badge" />
</p>

---

## 📊 GitHub Stats

<p align="center">
  <img 
    src="https://github-readme-stats.vercel.app/api?username=Donghwan814&theme=tokyonight&show_icons=true&hide_border=true&count_private=true&title_color=7C3AED&icon_color=7C3AED" 
    height="170" 
  />
  <img 
    src="https://github-readme-stats.vercel.app/api/top-langs/?username=Donghwan814&layout=compact&theme=tokyonight&hide_border=true&langs_count=8&card_width=350" 
    height="170" 
  />
</p>

<p align="center">
  <img 
    src="https://github-readme-activity-graph.vercel.app/graph?username=Donghwan814&theme=tokyo-night&hide_border=true&radius=12&area=true" 
    width="850" 
  />
</p>

---

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=Donghwan814&label=Profile%20views&color=7C3AED&style=for-the-badge" />
</p>

<p align="center">
  <img 
    src="https://capsule-render.vercel.app/api?type=waving&color=0:764ba2,50:7C3AED,100:667eea&height=130&section=footer" 
  />
</p>
