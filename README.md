# ⚡노승찬 | Back-end Developer

### “꾸준히 배우고, 쉽게 소통하며, 깊이 고민하고 개선하는 개발자”
> **꾸준하게 배우고 나만의 언어로 쉽게 설명하며, 모니터링과 검증을 통해 시스템 안정성과 성능을 고민하는 개발자.**

## 🙋‍♂️ 소개
- **유지보수가 쉬운 SW**를 개발하고 싶어요.
- 개발 과정에서 항상 **사용자의 입장**을 생각해요.
- 개발을 하나도 모르는 사람에게 **설명하고 이해 시키는 과정**에 자신 있어요.
- 모든 모니터링과 성능 개선은 **수치**를 통해 확인하고 검증해요.

<br/>

## 🎯 Focus Areas
> **"보이지 않는 곳에서 시스템을 단단하게 지탱합니다."**  
> 복잡한 대량의 비즈니스 데이터를 다루는 **Spring Batch 스케줄링**, 대규모 트래픽을 견디는 **성능 분석 및 튜닝**, 그리고 빈틈없는 **인프라 설계**에 큰 흥미를 느끼고 깊게 몰입합니다.

<br/>

## 🚀 Featured Project: NEXUS
> **가맹점-본사 통합 SCM 솔루션 (Backend)**  
> *본사와 가맹점 간의 복잡한 물류·재무 데이터를 무결하게 통합하고, 이벤트 기반의 시스템 동기화와 고성능 데이터 집계 엔진을 구축했습니다.*

### **🔑 핵심 도메인별 기술적 성과**

#### **1️⃣ 자동 정산 및 재무 파이프라인 (`billing`, `headincome`, `storeincom`)**
* **토스페이먼츠 연동 정기 결제 엔진**: 매월 10일 전월 미결제 내역을 자동 취합하여 결제하는 스케줄러 구축. 루프 내 개별 트랜잭션 격리를 통해 특정 가맹점 결제 실패가 전체 배치에 영향을 주지 않도록 설계.
* **고성능 매출 집계 및 N+1 문제 해결**: 가맹점 POS 매출 조회 시, 주문 아이템과 메뉴 데이터를 메모리 기반 그룹핑 전략으로 처리하여 DB 부하 최소화 및 응답 속도 최적화.
* **본사-가맹점 정산 데이터 무결성 보장**: 발주건 기반 본사 수입(`headincome`)과 판매건 기반 가맹점 매출(`storeincome`) 데이터를 정밀하게 동기화하여 투명한 정산 리포트 제공.

#### **2️⃣ 이벤트 기반 SCM 마스터 데이터 관리 (`product`, `category`)**
* **Kafka 기반 도메인 이벤트 발행**: 제품 정보 변경 시 Kafka 이벤트를 발행하여 타 도메인(재고, 발주 등)과의 결합도를 낮추고 비동기적 데이터 일관성을 유지하는 아키텍처 설계.
* **계층적 카테고리 구조 설계**: 물류 효율화를 위한 제품 분류 체계를 구축하고, 페이징 처리를 포함한 필터링 조회 API를 통해 대규모 제품군 관리 편의성 제공.

#### **3️⃣ 물류 생명주기 및 알림 자동화 (`delivery`)**
* **배송 상태 관리**: 발주 확정 시 자동으로 배송 데이터를 생성하고, 상태 변화를 enum으로 관리 (`READY` → `START` → `delivering` → `DELIVERED` → `DELAY`)에 따른 워크플로우 자동화 구현.
* **실시간 물류 알림 시스템**: 본사 배송 시작 시점에 맞춰 가맹점주에게 실시간 알림을 발송하여 물류 가시성 확보.

#### **4️⃣ 시스템 성능 및 보안 검증**
* **Spring Security & JWT 이중 인증 구축**: Cookie 기반(웹)과 Header 기반(API) 인증을 동시에 지원하는 필터 체인을 구축하여 다양한 클라이언트 환경 대응.
* **nGrinder 기반 부하 테스트**: 복잡한 인증 환경에서 고성능 부하 테스트를 수행하기 위해 Groovy 기반 동적 토큰 추출 및 헤더 주입 스크립트 설계.

<br/>

## 🛠️ Tech Stack

| 분류 | 기술 스택 (Stack) |
|:---:|---|
| **Language** | <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=OpenJDK&logoColor=white"/> |
| **Back-end** | <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=SpringBoot&logoColor=white"/> <img src="https://img.shields.io/badge/Spring_Batch-6DB33F?style=flat-square&logo=Spring&logoColor=white"/> |
| **Front-end** | <img src="https://img.shields.io/badge/Vue.js_3-4FC08D?style=flat-square&logo=Vue.js&logoColor=white"/> <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=HTML5&logoColor=white"/> <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=CSS3&logoColor=white"/> <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=React&logoColor=black"/> |
| **Database** | <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=white"/> <img src="https://img.shields.io/badge/MariaDB-003545?style=flat-square&logo=MariaDB&logoColor=white"/> |
| **DevOps** | <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=Kubernetes&logoColor=white"/> <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=Docker&logoColor=white"/> <img src="https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=Jenkins&logoColor=white"/> |
| **Test / Monitoring** | <img src="https://img.shields.io/badge/nGrinder-111111?style=flat-square&logo=micro-dot-blog&logoColor=white"/> <img src="https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=Postman&logoColor=white"/> <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=Prometheus&logoColor=white"/> <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=Grafana&logoColor=white"/> |
| **Version Control / Collaboration** | <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=Git&logoColor=white"/> <img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=GitHub&logoColor=white"/> |
| **Communication** | <img src="https://img.shields.io/badge/Discord-5865F2?style=flat-square&logo=Discord&logoColor=white"/> <img src="https://img.shields.io/badge/Slack-4A154B?style=flat-square&logo=Slack&logoColor=white"/> <img src="https://img.shields.io/badge/Notion-000000?style=flat-square&logo=Notion&logoColor=white"/> |

<br/>

## 🏅 Certifications & Milestones
* **SQLD (SQL 개발자)** | *한국데이터산업진흥원 (2026.09 취득)*
* **정보처리산업기사** | *한국산업인력공단 (2025.12 취득)*

<br/>

<p align="center">
  <span style="font-size: 60px; font-weight: 900;">지속 가능한 성장과 신뢰할 수 있는 개발을 추구합니다.</span><br/>
  📧 Email: <code>(shtmdcks06@gmail.com)</code>
</p>
