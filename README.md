<div align="center">

# Jayant Bhatia

### AI Systems & Backend Engineer

**Agentic AI · RAG · Python · FastAPI · Multi-Agent Systems**

<br>

<a href="https://github.com/jayant132"><img src="https://img.shields.io/badge/GitHub-jayant132-2b2b2b?style=for-the-badge&logo=github&logoColor=14B8A6" /></a>
<a href="https://www.linkedin.com/in/jayantbhatiaa"><img src="https://img.shields.io/badge/LinkedIn-Connect-2b2b2b?style=for-the-badge&logo=linkedin&logoColor=14B8A6" /></a>
<a href="mailto:jayantbhatia44@gmail.com"><img src="https://img.shields.io/badge/Email-Reach_Out-2b2b2b?style=for-the-badge&logo=gmail&logoColor=14B8A6" /></a>

</div>

<br>

<div align="center">

*I build the layer between an LLM and something people can actually rely on — retrieval that's grounded, agents that fail safely, and backend systems instrumented enough that when something's slow, I can find out why instead of guessing.*

**The model call is the easy part. The engineering happens everywhere around it.**

</div>

<br>

<div align="center">

<img src="https://skillicons.dev/icons?i=python,fastapi,postgres,redis,docker,githubactions,flutter,react,git&theme=dark" />

</div>

<br><br>

## 🧩 Flagship Builds

*Every project below reports a number, not an adjective — measured, not estimated.*

<br>

### 🛰️ Agentic Compliance Copilot
Assesses compliance readiness against internal policy documents — identifies gaps, assigns risk, and routes high-risk findings to a human for approval before anything is finalized.

Four agents coordinate through an explicit LangGraph state machine: an **Evidence Agent** runs as its own FastAPI process and is called over HTTP (a real agent-to-agent network boundary, not a function call), a **Risk & Gap Agent** classifies findings, and a **Critic Agent** reviews them for overreach. A deterministic guardrail — not an LLM grading its own homework — blocks any finding that cites a source outside what was actually retrieved.

| Metric | Result |
|:--|:--:|
| Retrieval accuracy | **20 / 20 (100%)** |
| Groundedness pass rate | **19 / 20 (95%)** |
| Hallucination rate | **1 / 20 (5%)** |
| Avg latency / case | **8,228 ms** |

**Real fix, found by reading the metrics, not guessing:** instrumentation showed the retrieval step re-creating a Pinecone client on every single call. Caching it at module load cut retrieval latency by **~37%** (9,200 ms → 5,784 ms).

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/> <img src="https://img.shields.io/badge/Google_ADK-4285F4?style=flat-square&logo=google&logoColor=white"/> <img src="https://img.shields.io/badge/LangGraph-1C1C1C?style=flat-square"/> <img src="https://img.shields.io/badge/Pinecone-000000?style=flat-square"/> <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/> <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>

**→ [View repository](https://github.com/jayant132/Agentic-Compliance-Copilot)**

<br>

### 🔎 DELVE — Deep Evidence & Log Verification Engine
An AI incident-investigation platform. Give it a plain-English incident description; it dispatches specialized agents to pull evidence from logs, metrics, deployments, and historical incidents **in parallel**, then synthesizes a root-cause hypothesis — labeled `low`/`medium`/`high` confidence, never presented as a confirmed fact. Nothing auto-executes without human approval.

| Step | Observed Latency |
|:--|:--:|
| Triage | **~2–4 s** |
| Full investigation (9 LLM calls, 4 parallel agents) | **~25–45 s** |
| Historical-incident retrieval (local ChromaDB) | **< 100 ms** |

**Proof the retrieval is actually semantic, not keyword-matching:** given a payment-service DB-pool-exhaustion incident, it correctly ranked the matching historical postmortem first — and correctly ranked a same-service-but-different-cause incident lower.

Built entirely on a free-tier stack (Groq, ChromaDB, local embeddings) with CI on every push, and ships an honest "known limitations" section rather than hiding them.

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/> <img src="https://img.shields.io/badge/Google_ADK-4285F4?style=flat-square&logo=google&logoColor=white"/> <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/> <img src="https://img.shields.io/badge/ChromaDB-6E56CF?style=flat-square"/> <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/>

**→ [View repository](https://github.com/jayant132/Delve-Deep-Evidence-Log-Verification-Engine-)**

<br>

### 🗣️ SQL AGENT LLM
Natural language in, a safe executed query out. Translates plain-English questions into SQL, executes them, and returns results — real tool-calling discipline applied to an everyday agentic workflow.

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/> <img src="https://img.shields.io/badge/LLM_Tool_Calling-14B8A6?style=flat-square"/> <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white"/>

**→ [View repository](https://github.com/jayant132/Sql_Agent_llm)**

<br>

### ✈️ Multi-Agent Flight Booking Assistant
One orchestrator delegates to three scoped agents — search, booking, support — instead of forcing a single model to hold the entire workflow in one context window.

| Agent | Scope |
|:--|:--|
| `SEARCH_AGENT` | Flight lookup tools |
| `BOOKING_AGENT` | Reservation tools |
| `SUPPORT_AGENT` | Post-booking tools |

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/> <img src="https://img.shields.io/badge/Multi--Agent_Orchestration-14B8A6?style=flat-square"/>

**→ [View repository](https://github.com/jayant132/Multi-Agent-AI-Flight-Booking-Assistant-)**

<br><br>

## 📦 Also Shipped

| Project | What it does | Stack |
|:--|:--|:--|
| **[Agentic Red Team Framework](https://github.com/jayant132/Agentic-Red-Team-Framework)** | Attacks tool-using agents across 7 classes; CI-gated at an 85% defended-pass threshold | Python · Ollama · pytest |
| **[MCP Guardrail](https://github.com/jayant132/MCP-Guardrail)** | Tests the MCP tool-catalog trust boundary directly | Python · MCP Protocol |
| **[Invoice Intelligence](https://github.com/jayant132/Invoice-Intelligence-ML-Project)** | One engineered feature took flagged-invoice recall from **17% → 99%** | Scikit-learn · Pandas |
| **[Tuberculosis Detection ML](https://github.com/jayant132/Tuberculosis-Detection-ML)** | Chest X-ray classification with a real pipeline structure | Computer Vision |
| **[JPMorgan Forage — Quant Research](https://github.com/jayant132/-JP-Morgan-Quantitative-Research-Virtual-Internship)** | JPMorgan Chase's official Forage quant-research simulation | Applied Quant Research |

<br><br>

## 🧱 System Architecture

| Layer | Tech |
|:--|:--|
| **Application** | Flutter · React Native · Web |
| **Backend** | FastAPI · AsyncIO · REST / WebSocket |
| **AI / Agents** | LLMs · RAG · LangGraph · Google ADK · Tool Calling |
| **Data** | PostgreSQL · pgvector · ChromaDB · Redis |

**The rule I hold to:** business logic stays deterministic. The LLM only runs where reasoning or generation is doing work an `if` statement can't — and every claim an agent makes should trace back to something it can point to.

<br><br>

## ⚙️ Stack

| Domain | Tools |
|:--|:--|
| **AI / Agentic** | LangGraph · Google ADK · LangChain · RAG · Tool Calling · Multi-Agent Orchestration |
| **AI Reliability** | Deterministic guardrails · Groundedness evaluation · Human-in-the-loop approval · Observability |
| **Backend** | Python · FastAPI · AsyncIO · REST · WebSockets · SSE |
| **Data** | PostgreSQL · pgvector · ChromaDB · Redis · MySQL · SQLite |
| **ML** | Scikit-learn · XGBoost · Pandas · NumPy |
| **Infra** | Docker · Docker Compose · GitHub Actions |

<br><br>

<div align="center">

### Open to AI Engineering & Backend Engineering roles
**Remote-friendly · Open to relocation**

<a href="https://github.com/jayant132"><img src="https://img.shields.io/badge/GitHub-jayant132-2b2b2b?style=for-the-badge&logo=github&logoColor=14B8A6" /></a>
<a href="https://www.linkedin.com/in/jayantbhatiaa"><img src="https://img.shields.io/badge/LinkedIn-Connect-2b2b2b?style=for-the-badge&logo=linkedin&logoColor=14B8A6" /></a>
<a href="mailto:jayantbhatia44@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-2b2b2b?style=for-the-badge&logo=gmail&logoColor=14B8A6" /></a>

</div>
