<!-- HEADER -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:1a1a2e,100:16213e&height=220&section=header&text=Rohit%20Saxena&fontSize=65&fontColor=00d4ff&animation=fadeIn&fontAlignY=38&desc=Backend%20Engineer%20%7C%20Distributed%20Systems%20%7C%20Cloud%20Infrastructure&descSize=18&descAlignY=62&descColor=8b949e"/>

<div align="center">

<a href="https://readme-typing-svg.demolab.com">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=16&duration=3000&pause=1000&color=00D4FF&center=true&vCenter=true&width=650&lines=Building+NexusPlatform+%E2%80%94+1M%2B+orders%2Fday+on+AWS+EKS;CQRS+%7C+Event+Sourcing+%7C+Saga+%7C+Redlock+%7C+Kafka;Go+%7C+Kubernetes+%7C+Terraform+%7C+Istio+%7C+OpenTelemetry;SDET+%40+Cognizant+%7C+Ex-ISRO+%7C+Ex-DRDO" alt="Typing SVG" />
</a>

<br/><br/>

[![Email](https://img.shields.io/badge/rohitsaxenaa08%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:rohitsaxenaa08@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Rohit_Saxena-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/rohit-saxena)
[![Portfolio](https://img.shields.io/badge/Portfolio-RohitGit0808.github.io-00d4ff?style=flat-square&logo=github&logoColor=white)](https://RohitGit0808.github.io)
[![Views](https://komarev.com/ghpvc/?username=RohitGit0808&style=flat-square&color=00d4ff&label=Profile+Views)](https://github.com/RohitGit0808)

</div>

<br/>

---

## About

I'm a **Backend & Distributed Systems Engineer** transitioning from enterprise test automation at Cognizant. I design and build cloud-native systems — microservices on Kubernetes, event-driven architectures on Kafka, infrastructure on AWS via Terraform.

My background combines software research (ISRO, DRDO) with production-grade engineering (CI/CD, observability, chaos testing). I build systems that are **scalable, observable, and resilient by design**.

```
Currently building  →  NexusPlatform (distributed commerce backend, 1M+ orders/day)
Open to             →  Backend Engineer · Platform Engineer · SRE
Location            →  Pune, India
```

---

## Flagship Project

<table>
<tr>
<td width="65%">

### [NexusPlatform](https://github.com/RohitGit0808/nexus-platform) — Distributed Commerce Backend

Production-grade event-driven microservices platform designed for **1M+ orders/day**.

**Distributed Patterns Implemented:**
- **Saga Orchestrator** — distributed transactions without 2-Phase Commit
- **CQRS + Event Sourcing** — separate read/write models, full audit trail, snapshots
- **Redlock Algorithm** — distributed mutex on 3 Redis nodes (majority quorum)
- **Sliding-window Rate Limiter** — atomic Lua scripts across all gateway replicas
- **Circuit Breaker** — per-upstream state machine (CLOSED → OPEN → HALF-OPEN)
- **Outbox Pattern** — guaranteed event delivery, no dual-write problem

**Infrastructure:**
- AWS EKS + MSK (Kafka) + RDS × 3 + ElastiCache — Terraform modules
- Istio mTLS + progressive canary delivery (10% → observe → 100%)
- HPA with custom metrics, PodDisruptionBudget, Chaos Engineering tests
- OpenTelemetry traces + Prometheus SLO alerts + Grafana dashboards

</td>
<td width="35%" align="center">

```
┌─────────────────────┐
│   API Gateway       │
│  JWT · RateLimit    │
│  CircuitBreaker     │
└────────┬────────────┘
         │
    ┌────┴─────┬──────┐
    ▼          ▼      ▼
 Order    Inventory Payment
 CQRS     Redlock   Idempotency
 Saga     Lock      Exactly-once
    │          │      │
    └────┬─────┴──────┘
         ▼
      Kafka
  nexus.orders
  nexus.payments
         │
         ▼
  Notification
   Service
```

</td>
</tr>
</table>

---

## Technical Skills

<div align="center">

| Domain | Technologies |
|--------|-------------|
| **Languages** | ![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) |
| **Distributed Systems** | ![Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=flat-square&logo=apache-kafka&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![gRPC](https://img.shields.io/badge/gRPC-4285F4?style=flat-square&logo=google&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) |
| **Cloud & Infra** | ![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white) ![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white) ![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Istio](https://img.shields.io/badge/Istio-466BB0?style=flat-square&logo=istio&logoColor=white) ![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white) |
| **Observability** | ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white) ![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white) ![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=flat-square&logo=opentelemetry&logoColor=white) ![Jaeger](https://img.shields.io/badge/Jaeger-60D0E4?style=flat-square) |
| **Testing & CI/CD** | ![Playwright](https://img.shields.io/badge/Playwright-45ba4b?style=flat-square&logo=playwright&logoColor=white) ![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white) |

</div>

---

## Projects

<div align="center">

| Repository | Description | Stack |
|------------|-------------|-------|
| [**nexus-platform**](https://github.com/RohitGit0808/nexus-platform) | Distributed commerce backend — CQRS, Event Sourcing, Saga, Redlock, Kafka, Canary deploys | `Go` `Kafka` `K8s` `Terraform` `AWS` `Istio` |
| [**playwright-ultimate-enterprise**](https://github.com/RohitGit0808/playwright-ultimate-enterprise) | Enterprise automation — 8 test types, BDD/Cucumber, Visual, A11y, Security, 4-shard CI | `TypeScript` `Playwright` `Cucumber` `Docker` |
| [**selenium-enterprise-framework**](https://github.com/RohitGit0808/selenium-enterprise-framework) | Java automation — Selenium Grid, TestNG, Allure, Cucumber BDD, multi-browser CI | `Java` `Selenium 4` `TestNG` `Allure` |
| [**Academic-Alleway-Integrated-with-AI**](https://github.com/RohitGit0808/Academic-Alleway-Integrated-with-AI) | AWS serverless ERP — Lambda, DynamoDB, EventBridge, SQS, AI chatbot, React | `AWS` `React` `DynamoDB` `Lambda` |
| [**FlockX**](https://github.com/RohitGit0808/FlockX) | Twitter clone — Spring Boot microservices, Spring Cloud, PostgreSQL, AWS S3, JWT | `Spring Boot` `Spring Cloud` `PostgreSQL` |
| [**Drone Navigation System**](https://github.com/RohitGit0808/Advance-Autonomous-Navigation-System-for-drone) | AI autonomous drone — TensorFlow, Dijkstra path planning, AirSim & Gazebo simulation | `Python` `TensorFlow` `PyTorch` |

</div>

---

## GitHub Stats

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=RohitGit0808&show_icons=true&theme=github_dark&include_all_commits=true&count_private=true&hide_border=true&title_color=00d4ff&icon_color=00d4ff&text_color=8b949e&bg_color=0D1117"/>
&nbsp;&nbsp;
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=RohitGit0808&layout=compact&theme=github_dark&hide_border=true&title_color=00d4ff&text_color=8b949e&bg_color=0D1117&langs_count=8"/>

</div>

<div align="center">
<img src="https://github-readme-streak-stats.herokuapp.com/?user=RohitGit0808&theme=github-dark-blue&hide_border=true&background=0D1117&ring=00d4ff&fire=ff6e00&currStreakLabel=00d4ff&sideLabels=8b949e&dates=8b949e"/>
</div>

<br/>

<div align="center">
<img src="https://github-readme-activity-graph.vercel.app/graph?username=RohitGit0808&theme=github-compact&hide_border=true&bg_color=0D1117&color=00d4ff&line=00d4ff&point=ff6e00&area=true&area_color=00d4ff"/>
</div>

---

## GitHub Trophies

<div align="center">
<img src="https://github-profile-trophy.vercel.app/?username=RohitGit0808&theme=darkhub&no-frame=true&no-bg=true&column=7&margin-w=4"/>
</div>

---

## Contribution

<div align="center">
<img src="https://raw.githubusercontent.com/RohitGit0808/RohitGit0808/output/github-contribution-grid-snake-dark.svg" alt="contribution snake"/>
</div>

---

## Experience

<div align="center">

| Company | Role | Period | Key Work |
|---------|------|--------|----------|
| **Cognizant** | SDET | May 2025 – Present | Enterprise automation frameworks · BDD · Dockerized CI/CD pipelines |
| **ISRO** | Software Intern | Jan – Jun 2024 | Validated NASA global aerosol datasets · Remote sensing data pipelines |
| **DRDO** | Software Intern | Mar – Aug 2022 | YOLOv3 military object detection model · **91.55% mAP** |

</div>

---

## Publications

<div align="center">

| Title | Venue | Status |
|-------|-------|--------|
| Efficient Pharmacy Tracker Application | ECS | ✅ Published |
| NLP Techniques in Customer Service | IEEE | 📖 Upcoming Book |

</div>

---

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:16213e,50:1a1a2e,100:0D1117&height=130&section=footer&animation=fadeIn"/>

<div align="center">

<sub>Open to Backend Engineer · Platform Engineer · SRE opportunities</sub>

[![Hire Me](https://img.shields.io/badge/Open_to_Work-00d4ff?style=for-the-badge&logo=gmail&logoColor=0D1117)](mailto:rohitsaxenaa08@gmail.com)

</div>
