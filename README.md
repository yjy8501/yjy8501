<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:F97316,100:FDBA74&height=200&section=header&text=%EC%96%91%EC%9E%AC%EC%9A%A9&fontSize=48&fontColor=ffffff&fontAlignY=36&desc=Backend%20Developer&descSize=20&descAlignY=58" width="100%" alt="양재용 · Backend Developer"/>

<img src="https://readme-typing-svg.demolab.com?font=Noto+Sans+KR&weight=600&size=20&pause=1800&color=F97316&center=true&vCenter=true&width=720&lines=%EC%8A%A4%ED%8E%99%EC%9C%BC%EB%A1%9C+%EB%A8%BC%EC%A0%80+%ED%95%A9%EC%9D%98%ED%95%98%EA%B3%A0%2C+AI%EB%A1%9C+%EA%B5%AC%ED%98%84%ED%95%98%EA%B3%A0%2C+%EA%B2%80%EC%A6%9D%EC%9C%BC%EB%A1%9C+%ED%92%88%EC%A7%88%EC%9D%84+%EC%A7%80%ED%82%B5%EB%8B%88%EB%8B%A4;%EB%8F%88%EA%B3%BC+%EB%8D%B0%EC%9D%B4%ED%84%B0%EA%B0%80+%EC%96%B4%EA%B8%8B%EB%82%98%EC%A7%80+%EC%95%8A%EB%8A%94+%EC%8B%9C%EC%8A%A4%ED%85%9C%EC%9D%84+%EB%A7%8C%EB%93%AD%EB%8B%88%EB%8B%A4" alt="스펙으로 먼저 합의하고, AI로 구현하고, 검증으로 품질을 지킵니다"/>

<a href="mailto:yjy850146@gmail.com"><img src="https://img.shields.io/badge/Email-yjy850146%40gmail.com-F97316?style=flat-square&logo=gmail&logoColor=white"/></a>
<a href="https://apps.apple.com/kr/app/%EA%B1%B0%EB%8B%90%EA%B0%95/id6809789351"><img src="https://img.shields.io/badge/App%20Store-%EA%B1%B0%EB%8B%90%EA%B0%95-0D96F6?style=flat-square&logo=appstore&logoColor=white"/></a>

</div>

## About

- **스펙 주도 개발 + AI** — 요구사항·검증 기준과 설계 결정(ADR)을 먼저 확정하고, AI로 구현한 뒤 스펙 대조 리뷰·정적 분석·통합 테스트로 검증합니다
- **결제 정합성** — 이중 결제 방지(조건부 갱신·승인 선점), API 멱등성 공통 계층, PG 연동, 정기결제 배치를 설계·구현했습니다
- **운영** — 사내에 없던 모니터링(Elastic APM)을 직접 구축해 장애와 슬로우 쿼리를 찾아 개선했고, 개인 서비스를 App Store에 출시해 운영하고 있습니다

## Tech Stack

<img src="https://skillicons.dev/icons?i=kotlin,java,spring,postgres,mysql,redis,aws,docker,nginx,githubactions,gradle" alt="Kotlin, Java, Spring, PostgreSQL, MySQL, Redis, AWS, Docker, nginx, GitHub Actions, Gradle"/>

![Spring AI](https://img.shields.io/badge/Spring%20AI-6DB33F?style=flat-square&logo=spring&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![QueryDSL](https://img.shields.io/badge/QueryDSL-0769AD?style=flat-square)
![Resilience4j](https://img.shields.io/badge/Resilience4j-333333?style=flat-square)
![Testcontainers](https://img.shields.io/badge/Testcontainers-291A3F?style=flat-square&logo=testcontainers&logoColor=white)
![Elastic APM](https://img.shields.io/badge/Elastic%20APM-005571?style=flat-square&logo=elastic&logoColor=white)

## Experience

| 기간 | 회사 | 한 일 |
|---|---|---|
| 2026.07 – 2026.11 | **오코랩스** · 백엔드 | 보안업체 S사 구독 서비스몰 결제·구독 백엔드 — 이중 결제 방지, 멱등성 공통 계층, PG 연동, 정기결제 배치, 환불 도메인 단독 설계 |
| 2024.08 – 2025.11 | **피피프렌즈** · 백엔드 | 반려동물 소셜 커뮤니티 API 서버 개발·운영 — 이벤트 기반 알림(API 응답 약 30% 개선), APM 모니터링 구축, 데드락·커넥션 풀 고갈 해결 |
| 2024.07 – 2024.08 | **Plea** · 백엔드 인턴 | Kafka·MSA 환경 경험, QR 요청 로그·엑셀 다운로드 API 개발 |

## Project — 거닐강

강원도 감성 키워드 기반 AI 여행 코스 추천 서비스 · 2026 한국관광공사 관광데이터 활용 공모전 출품 · 백엔드 1인 개발

- 골든셋 기반 검색 품질 평가 도구 — hit@10 97% → 질의 확장 적용 후 100%
- OpenAI Structured Output + 후보 장소 ID enum으로 LLM이 없는 장소를 지어내는 환각 차단
- TourAPI 일일 증분 동기화와 임베딩 입력 해시로 외부 호출·AI 비용 최소화
- 배포 후 자동 검증 — healthcheck → 설정 파일 대조 → 공개 URL 스모크 체크

<a href="https://apps.apple.com/kr/app/%EA%B1%B0%EB%8B%90%EA%B0%95/id6809789351"><img src="https://img.shields.io/badge/App%20Store-%EB%8B%A4%EC%9A%B4%EB%A1%9C%EB%93%9C-0D96F6?style=flat-square&logo=appstore&logoColor=white"/></a>
<a href="https://geonilgang-frontend.vercel.app"><img src="https://img.shields.io/badge/Web-%EB%B0%94%EB%A1%9C%EA%B0%80%EA%B8%B0-000000?style=flat-square&logo=vercel&logoColor=white"/></a>

<sub>서비스 운영 중이라 레포는 비공개입니다.</sub>

## Contributions

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/yjy8501/yjy8501/output/github-snake-dark.svg"/>
  <img src="https://raw.githubusercontent.com/yjy8501/yjy8501/output/github-snake.svg" alt="contribution snake"/>
</picture>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FDBA74,100:F97316&height=100&section=footer" width="100%"/>
