# Hi there, I'm Ankit 👋

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=2E9EF7&center=true&vCenter=true&width=600&lines=Senior+Software+Engineer;Workflow+%26+Approval+Systems+%7C+AI+Agents;Distributed+Systems+%7C+Microservices;5%2B+Years+Production+Experience;Based+in+Nepal+%F0%9F%87%B3%F0%9F%87%B5" alt="Typing SVG" />
</div>

## About Me

Senior Software Engineer with **5+ years** shipping production systems at scale. I specialize in workflow/approval engines, document orchestration pipelines, and distributed data processing, and I use AI tools (Claude Code, Gemini) as a core part of my daily engineering workflow, now extending into building agentic AI systems myself.

- **Currently:** Senior Engineer (mentoring role) at Progressive Labs, architecting the workflow and approval systems behind a fintech platform processing 50K+ daily transactions
- **Expertise:** Workflow state machines, approval/document orchestration engines, distributed systems, PostgreSQL at scale, applied AI/agentic systems
- **Open to:** Senior/Lead roles, technical leadership, system design challenges
- **Location:** Kathmandu, Nepal · UTC+5:45 · Remote-friendly

---

## Technical Stack

```yaml
Backend:      Node.js (5+ yrs) • NestJS • Express • TypeScript • Java (Spring Boot) • Python (FastAPI)
Workflow:     State Machines • Approval Engines • Orkes Conductor • Document Orchestration • Audit Trails
Data:         PostgreSQL (query optimization, JSONB, materialized views) • Neo4j (graph/Cypher) • MongoDB • Redis
Messaging:    Apache Kafka • BullMQ • AWS SQS/SNS
Cloud:        AWS (Fargate, EKS, RDS, S3, Lambda, KEDA) • GCP • Docker • Kubernetes • Terraform
Integrations: Braintree/PayPal • Plaid/Dwolla • webhook handling • API contract design
DevOps:       GitHub Actions • Flux • ArgoCD • blue-green deploys • PagerDuty • Sentry
Testing:      Jest • Vitest • Cypress • Testcontainers
AI / ML:      Gemini API • Multi-Agent Orchestration • MCP (Model Context Protocol) • Hybrid Search & RAG
              • LLM-as-Judge Evals • Claude Code (daily driver)
```

---

## Professional Experience

### Senior Software Engineer (Mentoring Role), Progressive Labs
*Sep 2024 – Present · Kathmandu, Nepal*

- **Approval & Workflow Engine** – Architected an approval/workflow engine handling bulk operations across millions of entities: clustering-based coordination without row-level locking, hierarchical state management, real-time state transitions, and full audit logging
- **Multi-Tenant Billing System** – Built a transaction-lifecycle state machine (pending, approved, settled, reconciled) for a payments platform processing 50K+ daily transactions at 99.95% uptime, integrating Braintree/PayPal for payments and Plaid/Dwolla for banking
- **Document Orchestration Pipeline** – Designed a distributed export pipeline (AWS Fargate, S3, SQS, KEDA, Orkes Conductor) rendering and delivering 100K+ PDFs/hour with idempotent, retryable processing and template-driven rendering across multiple layouts
- **PostgreSQL at Scale** – Cut critical query latency from 15s to 800ms through execution-plan analysis, GIN indexing, JSONB optimization, and materialized views
- **Engineering Culture** – Established an 85%+ test coverage standard, mentored engineers, led code reviews and architecture decisions, and use Claude Code/AI tools daily as part of the workflow
- 🏆 **Employee of the Quarter, Q4 2024**

### Software Engineer, Proshore / PowerLedger
*Sep 2022 – Jul 2024 · Kathmandu, Nepal*

- **Blockchain Energy Platform (TraceX)** – Developed full-stack features end-to-end across React frontends and Node.js/Spring Boot backends
- **Kafka Event Streaming** – Real-time pipeline from an internal registry through a gRPC blockchain adapter to Solana, with at-least-once delivery semantics, idempotency, and sub-second latency at millions of ops/day
- **Zero-Downtime Migration** – Migrated millions of records from Ethereum to Solana with 100% availability maintained throughout
- **GraphQL Federation** – Apollo Federation gateway across distributed Java microservices with backward-compatible schema composition
- **CI/CD & Velocity** – GitHub Actions + GCP cut deployment time 70%; led a monorepo decomposition that boosted release velocity 3x; Cypress E2E suite reached 85% regression coverage
- 🏆 **Spark of the Month, 2023**

### Backend Engineer, Code Himalaya
*May 2022 – Aug 2022 · Lalitpur, Nepal*

- Built a WebSocket infrastructure template for real-time interactions, cutting feature delivery time 60% through reusable patterns
- Implemented OAuth 2.0 + JWT authentication and scheduling systems with a security-first design
- Built an automated email warmup pipeline, improving domain reputation and inbox deliverability rates 40%

### Junior Software Engineer, TechKilla Technologies
*Nov 2020 – Jun 2021 · New Delhi, India*

- Built core components for a virtual event platform supporting 1K+ concurrent users, plus game mechanics (Minimax/Alpha-Beta Tic-Tac-Toe, pathfinding visualizer)

---

## Projects

### [AI Incident Response Copilot](https://github.com/bro-ankit/ai-incident-response-copilot)
Multi-agent incident investigation system · NestJS · CQRS · Gemini · MCP · Neo4j · pgvector

- Four specialized agents (log analysis, runbook search, root-cause synthesis, remediation) coordinated by an orchestrator, each reaching its tools through real MCP servers over stdio
- Service-dependency blast-radius lookups via Neo4j/Cypher, feeding remediation risk assessment
- Graceful degradation on sub-agent failure/timeout (retry, circuit breaker, timeout), partial results with explicit warnings instead of a hard failure
- LLM-as-judge eval harness scoring correctness and groundedness against a seeded golden set: 0.96 avg correctness, 1.00 avg groundedness

### [Smart Semantic Bookmarking & Memory Engine](https://github.com/bro-ankit/smart-semantic-booking-and-memory-engine)
Production-grade RAG system for knowledge management · NestJS · CQRS · Gemini · pgvector · BullMQ · Puppeteer

- URL ingestion with Readability, falling back to Puppeteer for JS-heavy sites
- Cosine similarity semantic search over pgvector embeddings, fused with keyword search and reranking
- Hallucination-resistant Q&A with structured, Zod-validated LLM outputs
- Retry logic, circuit breakers, dead-letter queue handling

### [Campus Placement Data Pipeline](https://github.com/bro-ankit/campus-placement-pipeline)
Enterprise Databricks lakehouse pipeline with ML predictions · PySpark · Delta Lake · scikit-learn · FastAPI

- Medallion architecture (Bronze/Silver/Gold) with per-layer data validation
- 30-feature Random Forest model for placement outcome prediction served via FastAPI
- Structured logging, data quality checks, dead-letter quarantine

### [To Games, Algorithm Visualizers](https://bro-ankit.github.io/toGames/)
Interactive algorithm demos: Minimax Tic-Tac-Toe, DFS pathfinding visualizer · JavaScript · Canvas API

---

## Open Source

### [pnpm](https://github.com/pnpm/pnpm) (contributor)
Fixed an auth config bug affecting multiple parts of the package manager, merged into a project used by millions of developers.
[github.com/pnpm/pnpm/pull/12679](https://github.com/pnpm/pnpm/pull/12679)

### [nestjs-typeorm-transactional-context](https://www.npmjs.com/package/@bro-ankit/nestjs-typeorm-transactional-context)
Production-grade NestJS library for type-safe transactional database operations, used in fintech and payment systems, 80+ weekly downloads.

---

## Writing

Technical deep dives on distributed systems, database optimization, and scaling: [medium.com/@jsankit99](https://medium.com/@jsankit99)

---

## Let's Connect

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ankit-pradhan-lm10/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bro-ankit)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jsankit99@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF6B6B?style=for-the-badge&logo=firefox&logoColor=white)](https://ankitpradhan.netlify.app/)
[![Medium](https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@jsankit99)

**Available for:** Contract work · Fullstack roles · System design · Technical consulting

</div>

---

<div align="center">

![Profile Views](https://komarev.com/ghpvc/?username=bro-ankit&color=58A6FF&style=flat-square)

*Building systems that scale, one production deployment at a time.*

</div>
