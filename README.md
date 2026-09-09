The reason the first lines failed to render on GitHub is that GitHub’s Markdown parser breaks when mixing raw HTML `div` tags with Markdown headers (`#`, `###`) without blank lines between them.

Here is the clean, 100% valid Markdown file. It uses pure HTML tags inside centered blocks and standard Markdown outside them so GitHub renders every badge, title, table, and ASCII diagram cleanly.

---

```markdown
<p align="center">
  <h1 align="center">JAYANT BHATIA</h1>
  <h3 align="center">AI Systems & Software Engineer</h3>
  <p align="center"><strong>Production GenAI · High-Throughput Backends · Cross-Platform Mobile & Web</strong></p>
  <p align="center">Building intelligent, end-to-end systems from model inference and data pipelines to resilient backend architectures and deployed client applications.</p>
</p>

<p align="center">
  <a href="https://github.com/jayant132">
    <img src="https://img.shields.io/badge/GitHub-jayant132-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
  <a href="https://www.linkedin.com/in/jayantbhatiaa">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:jayantbhatia44@gmail.com">
    <img src="https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=jayant132&label=PROFILE+VIEWS&color=39FF14&style=for-the-badge&labelColor=111111" alt="Profile Views" />
</p>

---

## > WHO I AM

I am an **AI Systems & Software Engineer** delivering solutions across three unified product layers:

1. **Generative AI & Agentic Systems:** Multi-agent orchestration, tool-calling loops, advanced RAG architectures, and automated evaluation harnesses.
2. **Backend & Distributed Systems:** Asynchronous REST backends, schema validation, Redis caching, event queues, and containerized deployments.
3. **Cross-Platform Client Engineering:** Shipped production applications on Android and iOS built with Flutter and React Native.

```text
┌─────────────────┐       ┌─────────────────┐       ┌─────────────────┐       ┌─────────────────┐
│   DATA & CACHE  │ ───►  │ AI REASONING /  │ ───►  │ BACKEND APIS &  │ ───►  │ MOBILE & CLIENT │
│   FOUNDATION    │       │ ML INFERENCE    │       │ MICROSERVICES   │       │ INTERFACES      │
├─────────────────┤       ├─────────────────┤       ├─────────────────┤       ├─────────────────┤
│ PostgreSQL      │       │ LangGraph       │       │ FastAPI         │       │ Flutter         │
│ pgvector        │       │ Ollama / Bedrock│       │ Pydantic        │       │ React Native    │
│ Redis           │       │ Scikit-Learn    │       │ Docker          │       │ WebSockets      │
│ SQLite          │       │ Google ADK      │       │ Celery / Queues │       │ State Mgmt      │
└─────────────────┘       └─────────────────┘       └─────────────────┘       └─────────────────┘

```

**I bridge the gap between machine intelligence and production engineering: writing the model logic, wrapping it in robust backends, and surfacing it to client users.**

---

## 01 — FEATURED PRODUCTION WORK

### ✈️ Multi-Agent Travel Assistant

**Collaborative agent orchestrator built on LangGraph & FastAPI.**
Coordinates flight lookups, hotel booking logic, and corporate travel policy compliance using state machines and external API tool integration.

`LangGraph` `FastAPI` `Tool Calling` `Groq` `Python`

### 🛡️ Agentic Red Team Framework

**CI/CD automated security harness testing OWASP Top 10 LLM risks.**
Attacks tool-enabled agents to detect prompt injection, tool hijacking, and excessive agency, enforcing regression passes prior to production shipping.

`AI Safety` `Threat Modeling` `CI Gates` `Docker` `Python`

### 🧾 Invoice Intelligence & Risk ML

**Dual-pipeline ML forecasting and fraud detection system.**
Estimates baseline freight logistics costs and flags suspicious discrepancies using custom feature engineering (`Dollar_Gap`), achieving a 99% audit recall rate.

`Scikit-Learn` `Pandas` `Feature Engineering` `SQLite` `Joblib`

### 📱 Full-Stack & Mobile Systems

**High-concurrency FastAPI backends connected to shipped mobile clients.**
Production REST and WebSocket services featuring Redis session caching, PostgreSQL sync, and cross-platform Flutter/React Native deployments on mobile stores.

`Flutter` `React Native` `FastAPI` `PostgreSQL` `Redis`

---

## 02 — CORE COMPETENCIES

### 🤖 Generative AI & Autonomous Agents

* **State Machine Orchestration:** Deterministic routing, cycles, and human-in-the-loop validation using LangGraph.
* **Retrieval-Augmented Generation (RAG):** Document indexing, hybrid semantic/BM25 retrieval, context compression, and grounding checks.
* **Tool Calling & Automation:** Schema-driven tool use using Pydantic and JSON Schema for reliable database writes and external API calls.
* **Adversarial Safety & Guardrails:** Prompt injection mitigation, deterministic input/output sanitizers, and continuous security evaluation.

### ⚙️ Backend & Systems Engineering

* **High-Concurrency APIs:** Asynchronous REST and streaming WebSocket services engineered with Python (FastAPI, Asyncio).
* **Data Layer & Validation:** Strict typing via Pydantic, relational database design in PostgreSQL/MySQL, and vector embeddings in `pgvector`.
* **State & Performance Caching:** Sub-millisecond session state management, caching, and rate limiting backed by Redis.
* **Production Reliability:** Automated testing suites (`pytest`), containerization with Docker Compose, and CI/CD automation via GitHub Actions.

### 📱 Cross-Platform Mobile & Frontend

* **Cross-Platform Native Apps:** Shipped production-ready mobile applications built with **Flutter** and **React Native**.
* **Real-Time Data Streaming:** Low-latency token streaming to UI interfaces via WebSockets and Server-Sent Events (SSE).
* **State Management & Offline Storage:** Predictable UI state flows (Bloc, Provider, Redux) coupled with SQLite/Hive for offline-first support.
* **Store Deployment:** Direct experience preparing builds, managing signing keys, and deploying to Google Play and Apple App Store.

### 🧠 Classical Machine Learning

* **Predictive Pipelines:** Exploratory data analysis, missing data imputation, normalization, and domain feature engineering.
* **Supervised Modeling:** Binary/multiclass classification and regression modeling with Scikit-Learn, Random Forests, and XGBoost.
* **Model Validation:** Precision-recall curve tuning, confusion matrix diagnostics, cross-validation, and Joblib model serialization.

---

## 03 — TECH STACK

---

## 04 — SYSTEM ARCHITECTURE WALKTHROUGHS

### ✈️ Multi-Agent AI Flight Booking Assistant

**Collaborative agent architecture orchestrating real-time travel planning, tool verification, and booking validation.**

```text
                               USER REQUEST
                                    │
                                    ▼
                         CENTRAL PLANNER AGENT
                        (State Machine Routing)
                                    │
           ┌────────────────────────┼────────────────────────┐
           ▼                        ▼                        ▼
     FLIGHT RETRIEVER          HOTEL FINDER             POLICY ENGINE
    (External Flight API)   (Dynamic Search Tool)   (Vector Store / RAG)
           │                        │                        │
           └────────────────────────┼────────────────────────┘
                                    ▼
                         VALIDATOR & GUARD AGENT
                        (Pydantic Schema Check)
                                    │
                                    ▼
                         FINAL STRUCTURED OUTPUT

```

* **Deterministic Orchestration:** Uses LangGraph to ensure multi-step workflows follow business validation paths rather than unpredictable loops.
* **Tool Calling & Guardrails:** Integrates custom API tools with input sanitization and fallback error recovery.
* **Production Boundary:** Wrapped in an asynchronous FastAPI backend, ready for consumption by Flutter or web clients.

[Explore the Flight Booking Assistant Repository →](https://github.com/jayant132/Multi-Agent-AI-Flight-Booking-Assistant-)

---

### 📱 Full-Stack Delivery: FastAPI Gateway to Cross-Platform Mobile

**Engineering the direct connection between AI backend inference and native client devices.**

```text
┌─────────────────────────────────┐
│     CLIENT APPS (IOS / ANDROID) │
│     Flutter  |  React Native    │
└────────────────┬────────────────┘
                 │ (Secure HTTPS / Streaming WSS)
┌────────────────▼────────────────┐
│     FASTAPI GATEWAY & WORKERS   │
│     Pydantic Validation / Auth  │
└───────┬─────────────────┬───────┘
        │                 │
┌───────▼───────┐ ┌───────▼───────┐
│  DATA STORES  │ │  AI SERVICES  │
│  Postgres /   │ │  Agents /     │
│  Redis Cache  │ │  RAG Pipeline │
└───────────────┘ └───────────────┘

```

* **Token Streaming:** Implemented WebSockets and SSE to stream chunk-by-chunk LLM token output directly to mobile screens for sub-second perceived response times.
* **Production Mobile Releases:** Engineered, built, and deployed applications to both the Apple App Store and Google Play Store.
* **Diagnostics & Tracing:** Integrated OpenTelemetry tracing across client request IDs, backend routes, and database/LLM execution spans.

---

### 🧾 Invoice Intelligence & Risk Forecasting

**End-to-end predictive ML pipeline resolving invoice variance, freight overcharging, and payment fraud.**

```text
Raw Invoice DB ──► Feature Engineering ──► Model Selection ──► Threshold Tuning ──► Audit Alert API
  (PostgreSQL/       (Gap Analysis,         (Random Forest,     (Precision-Recall     (FastAPI
    SQLite)           Transit Drift)          HistGradient)       Optimization)        Inference)

```

* **Feature Engineering Impact:** Designed the domain-specific `Dollar_Gap` feature, taking high-risk invoice anomaly recall from **17% to 99%**.
* **Inference Packaging:** Serialized models using Joblib, serving predictions via a lightweight FastAPI container running sub-50ms audit checks.

[Explore Invoice Intelligence Repository →](https://github.com/jayant132/Invoice-Intelligence-ML-Project)

---

## 05 — ENGINEERING PRINCIPLES

```text
┌─────────────────────────────────────────────────────────┐
│              PRAGMATIC SOFTWARE ENGINEERING             │
├─────────────────────────────────────────────────────────┤
│                                                         │
│   Resilient Data  ──►  Verified Logic  ──►  Clean UX    │
│         │                     │                  │      │
│   PostgreSQL /           FastAPI /          Flutter /   │
│   Schema Control         Agent State       React Native │
│                                                         │
└─────────────────────────────────────────────────────────┘

```

* **Deterministic First:** Use deterministic code for arithmetic, database queries, and business validations; use LLMs for natural language extraction, synthesis, and creative reasoning.
* **End-to-End Ownership:** An AI algorithm is only as useful as the backend hosting it and the client interface delivering it. I own the entire vertical slice.
* **Continuous Safety & Verification:** Integrate unit tests, latency benchmarks, and red-team security evals directly into the CI/CD pipeline before shipping to production.

---

## 06 — OPEN FOR COLLABORATION

I am open to discussions regarding:

* **AI Systems & GenAI Engineering Roles**
* **Backend Software Engineering (Python / FastAPI / Cloud Services) Roles**
* **Mobile & Full-Stack (Flutter / React Native / APIs) Roles**
