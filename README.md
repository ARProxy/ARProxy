[![Blog](https://img.shields.io/badge/❤️_Blog-hocci--0222.tistory.com-FF5722?style=flat-square)](https://hocci-0222.tistory.com)
[![Email](https://img.shields.io/badge/✉️_Email-kwon.donghwi22%40gmail.com-03A9F4?style=flat-square)](mailto:kwon.donghwi22@gmail.com)
[![LinkedIn](https://img.shields.io/badge/🔗_LinkedIn-donghwi-0A66C2?style=flat-square)](https://www.linkedin.com/in/arproxy/)

## 안녕하세요, 백엔드 개발자입니다 👋

### 하고 있는 일

- eKYC 신분증 인증 솔루션 1인 운영 및 고도화 (두나무 증권 상장 플러스 국내 첫 수주)
- Vision AI 기반 화면정보 보호 솔루션 개발 (삼성 계열사 내부망, 약 수만 명 규모)
- LLM/VLM/RAG 기반 이상행위 자동 분석 시스템 설계 (진행 중)
- 사내 소프트웨어 라이선스 관리 시스템(LMS) 신규 개발
- 가치관 기반 AI 매칭 소개팅 앱 Piece 백엔드 설계·운영 (사이드 프로젝트)

### eKYC 인증 솔루션

신분증 사본 판별·OCR·라이브니스·얼굴 1:1 매칭 기능을 제공하는 eKYC 솔루션 1인 운영

`Java 21` `Spring Boot 3.x` `MySQL` `Redis` `QueryDSL` `Resilience4j` `Prometheus` `Grafana` `Loki` `EKS`

- 응답 속도 40% 개선: 모듈 간 불필요한 왕복 호출 제거 + 모듈리스 전환 (p50: 1,440ms → 860ms)
- 장애 인지 30분 → 즉시: 단일 관측 지점 설계 + 어댑터 패턴 외부 호출 통합 + 수치 기반 알림 체계 구축
- 통합 대시보드: Prometheus + Grafana + Loki 기반, 시스템 상태 확인 10분 → 1분
- 신분증 OCR 정확도 87% → 96%: YOLO 자동 정렬 + CLAHE 6단계 전처리 + 국가별 특화 후처리
- 여권 NFC SDK 자체 개발 (iOS/Android): PACE/BAC 자동 폴백, 인식률 95%
- 외부 모듈 안정성 확보: Resilience4j 재시도 + Engine 어댑터 패턴으로 의존성 캡슐화
- 사업 성과: 중계사(쿠콘) 협업으로 두나무 증권 상장 플러스 국내 첫 수주, 금융권 PoC 확장 중

### Vision AI 기반 화면정보 보호 솔루션

삼성 계열사 내부망 VDI 기반 얼굴인식 보안 솔루션 개발

`Java 17` `Spring Boot 3.x` `MySQL` `Redis` `Elasticsearch` `Kafka`

- Redis Hash 기반 등록PC 캐싱: 다층 해시 필드 설계로 응답시간 150ms → 3ms (98% 개선), DB 커넥션 70% 감소
- 분산 서버 실시간 정책 동기화: Redis Pub/Sub + WebSocket(STOMP) + SockJS, 알림 지연 5초 → 100ms 이하
- IP 우회 공격 대응: OncePerRequestFilter + CIDR 기반 IP 검증 + Redis 세션 즉시 삭제
- LLM/VLM 기반 이상행위 자동 분석 시스템 설계 중 (하루 10만 건+ 이벤트 로그 자동 분석)

### 라이선스 관리 시스템

고객사 납품 소프트웨어 라이선스 통합 관리 시스템 신규 개발 | 서버 2명, 기여도 60%

`Java 17` `Spring Boot 3.x` `PostgreSQL` `Redis` `Redisson` `JPA` `Quartz` `JNI` `AWS ECS`

- 분산 환경 동시성 제어: 낙관적 락 → 비관적 락 → Redisson 분산 락, 중복 갱신 3~5건/일 → 0건
- 트랜잭션 격리: AFTER_COMMIT 이벤트 + REQUIRES_NEW로 이력 손실 방지
- JNI 기반 C++ 암호화 모듈 연동: RSA/AES256 12개 함수 래핑, Go 레거시 서버와 100% 호환
- 스케줄러 자동화: Quartz 기반 갱신·만료 알림·다국어 이메일 발송

### 사이드 프로젝트 — Piece (소개팅 앱)

사용자 500+, DAU 40 규모의 가치관 매칭 소개팅 앱 설계·구축·운영

`Java 21` `Spring Boot 3.2` `MySQL 8.0` `Redis` `Qdrant` `AWS CDK`

- 보안 사고 대응: 채굴 봇 해킹 → WAF-ALB-SG-Private Subnet 다계층 방어 + CDK 기반 IaC 전환
- 비용 최적화: NAT Instance 전환 + AWS 크레딧 $1,000 확보로 8개월 무료 운영
- 매칭 알고리즘 고도화: Gale-Shapley 기반 4단계 하이브리드 매칭 + 40~50차원 벡터 유사도

### 주의 깊게 학습하는 키워드

`JVM & GC` `운영체제` `데이터베이스(MySQL 내부 구조)` `분산 시스템` `네트워크` `알고리즘`


### 사이드 프로젝트
[**Piece**](https://github.com/Piece-Puzzly) - 가치관 기반 매칭 데이팅 앱 운영 중

### 💪 스킬

**Platforms & Languages**

![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)

**Database**

![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=flat-square&logo=mariadb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

**Infra & Tools**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
