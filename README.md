<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:F97316,100:FDBA74&height=200&section=header&text=%EC%96%91%EC%9E%AC%EC%9A%A9&fontSize=48&fontColor=ffffff&fontAlignY=36&desc=Backend%20Developer&descSize=20&descAlignY=58" width="100%" alt="양재용 · Backend Developer"/>

<img src="https://readme-typing-svg.demolab.com?font=Noto+Sans+KR&weight=600&size=20&pause=1800&color=F97316&center=true&vCenter=true&width=720&lines=%EC%8A%A4%ED%8E%99%EC%9C%BC%EB%A1%9C+%EB%A8%BC%EC%A0%80+%ED%95%A9%EC%9D%98%ED%95%98%EA%B3%A0%2C+AI%EB%A1%9C+%EA%B5%AC%ED%98%84%ED%95%98%EA%B3%A0%2C+%EA%B2%80%EC%A6%9D%EC%9C%BC%EB%A1%9C+%ED%92%88%EC%A7%88%EC%9D%84+%EC%A7%80%ED%82%B5%EB%8B%88%EB%8B%A4;%EB%8F%88%EA%B3%BC+%EB%8D%B0%EC%9D%B4%ED%84%B0%EA%B0%80+%EC%96%B4%EA%B8%8B%EB%82%98%EC%A7%80+%EC%95%8A%EB%8A%94+%EC%8B%9C%EC%8A%A4%ED%85%9C%EC%9D%84+%EB%A7%8C%EB%93%AD%EB%8B%88%EB%8B%A4" alt="스펙으로 먼저 합의하고, AI로 구현하고, 검증으로 품질을 지킵니다"/>

<a href="mailto:yjy850146@gmail.com"><img src="https://img.shields.io/badge/Email-yjy850146%40gmail.com-F97316?style=flat-square&logo=gmail&logoColor=white"/></a>
<a href="https://apps.apple.com/kr/app/%EA%B1%B0%EB%8B%90%EA%B0%95/id6809789351"><img src="https://img.shields.io/badge/App%20Store-%EA%B1%B0%EB%8B%90%EA%B0%95-0D96F6?style=flat-square&logo=appstore&logoColor=white"/></a>

</div>

## About

Kotlin · Spring 백엔드 개발자<br/>
결제·구독 서비스, 커뮤니티 서비스 백엔드 개발 · 개인 서비스 「거닐강」 운영 중

## How I Work

```mermaid
flowchart LR
    A["스펙 · ADR<br/>요구사항 · 검증 기준 · 설계 결정"] --> B["AI 구현<br/>Claude Code"]
    B --> C["자동 검증<br/>정적 분석 · 아키텍처 규칙 · 통합 테스트"]
    C --> D["스펙 대조 리뷰"]
    D -->|기준 미달| B
    D -->|통과| E["머지"]
```

- **스펙이 AI의 정답지** — 검증 기준이 없으면 AI는 요구사항을 추측해서 그럴듯하게 구현합니다. 그래서 구현보다 스펙을 먼저 씁니다
- **결정은 기록으로** — 대안과 기각 이유까지 ADR에 남겨, 요구사항이 바뀌어도 영향 범위를 추적합니다
- **AI의 오판은 규칙으로** — 틀린 판단은 작업 규칙으로 쌓아 같은 실수가 반복되지 않게 합니다
- **동시성은 실제로 경쟁시켜서** — 목(mock)이 아니라 실제 PostgreSQL·Redis에서 여러 스레드를 경쟁시켜 확인합니다

## Featured

### 거닐강 — 강원도 AI 여행 코스 추천

<a href="https://apps.apple.com/kr/app/%EA%B1%B0%EB%8B%90%EA%B0%95/id6809789351"><img src="https://img.shields.io/badge/App%20Store-%EB%8B%A4%EC%9A%B4%EB%A1%9C%EB%93%9C-0D96F6?style=flat-square&logo=appstore&logoColor=white"/></a>
<a href="https://geonilgang-frontend.vercel.app"><img src="https://img.shields.io/badge/Web-%EB%B0%94%EB%A1%9C%EA%B0%80%EA%B8%B0-000000?style=flat-square&logo=vercel&logoColor=white"/></a>

2026 한국관광공사 관광데이터 활용 공모전 출품 · App Store 출시 · 백엔드 1인 개발 <sub>(서비스 운영 중이라 레포는 비공개)</sub>

| 풀어낸 문제 | 방법 |
|---|---|
| 추천이 맞는지 감으로 판단하던 문제 | 골든셋 질의 37개로 검색 품질을 수치화 — hit@10 97% → 질의 확장 후 100% |
| LLM이 없는 장소를 지어내는 환각 | Structured Output + 후보 장소 ID enum으로 후보 밖 응답 자체를 차단 |
| 관광 데이터 갱신 비용 | 변경분만 동기화하고, 내용이 바뀐 장소만 임베딩 재계산 |
| 「배포 성공」인데 5일간 500이던 사고 | 배포 후 공개 URL 스모크 체크 — 상태코드로 실패 원인까지 구분 |

## Experience

- **오코랩스** · 백엔드 <sub>2026.07 – 2026.11</sub> — 보안업체 S사 구독 서비스몰. 이중 결제 방지, 멱등성 공통 계층, PG 연동, 정기결제 배치, 환불 도메인 단독 설계
- **피피프렌즈** · 백엔드 <sub>2024.08 – 2025.11</sub> — 반려동물 소셜 커뮤니티 API 개발·운영. 이벤트 기반 알림(응답 약 30% 개선), APM 모니터링 직접 구축, 데드락·커넥션 풀 고갈 해결

## Tech Stack

<img src="https://skillicons.dev/icons?i=kotlin,java,spring,postgres,mysql,redis,aws,docker,nginx,githubactions,gradle" alt="Kotlin, Java, Spring, PostgreSQL, MySQL, Redis, AWS, Docker, nginx, GitHub Actions, Gradle"/>

![Spring AI](https://img.shields.io/badge/Spring%20AI-6DB33F?style=flat-square&logo=spring&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![QueryDSL](https://img.shields.io/badge/QueryDSL-0769AD?style=flat-square)
![Resilience4j](https://img.shields.io/badge/Resilience4j-333333?style=flat-square)
![Testcontainers](https://img.shields.io/badge/Testcontainers-291A3F?style=flat-square&logo=testcontainers&logoColor=white)
![Elastic APM](https://img.shields.io/badge/Elastic%20APM-005571?style=flat-square&logo=elastic&logoColor=white)

## Contributions

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/yjy8501/yjy8501/output/github-snake-dark.svg"/>
  <img src="https://raw.githubusercontent.com/yjy8501/yjy8501/output/github-snake.svg" alt="contribution snake"/>
</picture>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FDBA74,100:F97316&height=100&section=footer" width="100%"/>
