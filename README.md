<div align="center">

# Jayant Bhatia

### AI Systems & Software Engineer

**Generative AI · Agentic AI · RAG · Python · FastAPI · Distributed Systems**

Building production-grade AI and software systems — from LLM-powered agents, RAG pipelines,
and model inference to scalable backend APIs, data systems, and cross-platform applications.

<p>
  <a href="https://github.com/jayant132">
    <img src="https://img.shields.io/badge/GitHub-jayant132-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  </a>
  <a href="https://www.linkedin.com/in/jayantbhatiaa">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="mailto:jayantbhatia44@gmail.com">
    <img src="https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
  </a>
</p>

<p>
  <img src="https://komarev.com/ghpvc/?username=jayant132&label=PROFILE+VIEWS&color=39FF14&style=for-the-badge&labelColor=111111" alt="Profile Views">
</p>

<br>

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/LangGraph-1C1C1C?style=flat-square&logo=langchain&logoColor=white"/>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white"/>
<img src="https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB"/>

</div>

<br>

## About Me

I'm a **Software Engineer focused on Generative AI, Agentic AI, backend engineering, and machine learning systems.**

My work spans the full lifecycle of AI-powered applications:

- **Generative AI & Agentic Systems** — LLM applications, RAG pipelines, multi-agent workflows, tool calling, structured outputs, and evaluation
- **Backend & API Engineering** — Python, FastAPI, async services, REST APIs, WebSockets, authentication, validation, caching, and database integration
- **Data & ML Engineering** — data preprocessing, feature engineering, model development, evaluation, inference pipelines, and model serving
- **Production Engineering** — Docker, CI/CD, automated testing, observability, and production-oriented system design
- **Application Development** — Flutter, React Native, and web apps integrated with AI and backend services

> My focus isn't only on building models or prototypes — it's on turning AI capabilities into
> **reliable software systems** that can be integrated, tested, deployed, and consumed by real applications.

<br>

## System Architecture

<table>
<tr><td align="center">📱&nbsp;&nbsp;<b>Application Layer</b><br/><sub>Flutter · React Native · Web</sub></td></tr>
<tr><td align="center">⬇️</td></tr>
<tr><td align="center">⚙️&nbsp;&nbsp;<b>Backend Layer</b><br/><sub>FastAPI · Python · Pydantic · AsyncIO · REST / WebSocket</sub></td></tr>
<tr><td align="center">⬇️</td></tr>
<tr><td align="center">🤖&nbsp;&nbsp;<b>AI / ML Layer</b><br/><sub>LLMs · RAG · LangGraph · Google ADK · Scikit-Learn</sub></td></tr>
<tr><td align="center">⬇️</td></tr>
<tr><td align="center">🗄️&nbsp;&nbsp;<b>Data Layer</b><br/><sub>PostgreSQL · Redis · pgvector · SQLite</sub></td></tr>
</table>

**Engineering approach:** combine deterministic software engineering with AI capabilities —
traditional code handles business rules, validation, and system control, while LLMs are used
where reasoning, language understanding, and generation provide measurable value.

<br>

## What I Build

<table>
<tr>
<td width="50%" valign="top">

### 🤖 Generative AI & Agentic Systems
Designing AI applications around LLMs, RAG, agents, and tool-enabled workflows.

- Multi-agent systems (LangGraph, state-based orchestration)
- Retrieval-Augmented Generation pipelines
- Vector search & semantic retrieval
- Tool calling & structured outputs (Pydantic / JSON Schema)
- Prompt engineering & context management
- LLM evaluation & regression testing
- Guardrails & prompt-injection defenses
- AI/LLM red-teaming & adversarial testing
- Local and cloud model inference

</td>
<td width="50%" valign="top">

### ⚙️ Backend & Distributed Systems
Building reliable backend services around AI and application logic.

- Python & FastAPI
- Async programming (AsyncIO)
- REST API design
- WebSockets & Server-Sent Events
- PostgreSQL / MySQL / SQLite
- Redis caching & state management
- Background workers & queues
- Docker, Docker Compose & CI/CD

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🧠 Machine Learning
End-to-end ML pipelines from data preparation through inference.

- Exploratory data analysis
- Data preprocessing & feature engineering
- Classification & regression
- Random Forest / gradient-boosting models
- Model evaluation & threshold optimization
- Precision / recall analysis & cross-validation
- Model serialization & inference APIs

</td>
<td width="50%" valign="top">

### 📱 Application Engineering
Connecting backend and AI services to production-grade clients.

- Flutter & React Native
- ReactJS
- REST API & WebSocket integration
- State management & local persistence
- Authentication
- Mobile app deployment

</td>
</tr>
</table>

<br>

## Featured Projects

<table>
<tr><td width="50%" valign="top">

### 🛡️ Agentic Red Team Framework
A production-shaped red-team harness for tool-using LLM agents.

- 4 tools attacked: web search, file system, database, external API
- 7 attacks: direct/indirect prompt injection, tool abuse, privilege escalation, data exfiltration, excessive agency
- 4-level outcome rubric (`BLOCKED` → `FULL_SUCCESS`), not pass/fail
- CI security gate — blocks merges below an 85% defended pass-rate threshold
- Benchmarked on two backends: a deterministic mock and a real local LLM (Ollama)

| Mode | Backend | Pass Rate |
|---|---|---|
| Baseline (no defenses) | Mock | 0/7 (0%) |
| Defended | Mock | 6/7 (86%) ✅ |
| Baseline (no defenses) | Ollama (llama3.2:1b) | 6/7 (86%) ✅ |
| Defended | Ollama (llama3.2:1b) | 7/7 (100%) ✅ |

**Stack:** Python · ReAct agent loop · Ollama · SQLite · pytest · GitHub Actions
**Mapped to:** OWASP Agentic AI threat categories

**Repo:** [github.com/jayant132/Agentic-Red-Team-Framework](https://github.com/jayant132/Agentic-Red-Team-Framework)

</td>
<td width="50%" valign="top">

### 🔐 MCP Guardrail
A security scanner for MCP (Model Context Protocol) servers and clients — testing the tool-catalog trust boundary that most AI red-team tooling skips.

- 5 attacks: tool-description poisoning, indirect injection via tool output, credential exposure, trust-boundary violation, allowlist bypass
- Same 4-level rubric and baseline-vs-defended discipline as the companion project above
- Defense-in-depth proven on a real run: a documented sanitizer gap (paraphrase evasion) caught by an independent allowlist layer
- CI security gate on every push

| Mode | Backend | Pass Rate |
|---|---|---|
| Baseline (no defenses) | Mock | 0/5 (0%) |
| Defended | Mock | 5/5 (100%) ✅ |
| Baseline / Defended | Ollama (llama3.2:1b) | 5/5 (100%) ✅ |

**Stack:** Python · MCP protocol · Ollama · pytest · GitHub Actions
**Mapped to:** OWASP GenAI LLM Top 10 (2026)

**Repo:** [github.com/jayant132/MCP-Guardrail](https://github.com/jayant132/MCP-Guardrail)

</td>
</tr>
</table>

> Both projects report real, reproducible numbers — including baselines proving the attacks work, and honestly-documented limitations rather than only "everything blocked" results.

<br>

## Engineering Stack

<table>
<tr><th align="left">Category</th><th align="left">Technologies</th></tr>
<tr><td><b>Generative AI</b></td><td>LLMs, RAG, Agentic AI, Prompt Engineering, Tool Calling</td></tr>
<tr><td><b>AI Frameworks</b></td><td>LangGraph, LangChain, Google ADK</td></tr>
<tr><td><b>AI Security</b></td><td>Prompt-injection defense, red-teaming, MCP trust-boundary testing, OWASP GenAI mapping</td></tr>
<tr><td><b>Backend</b></td><td>Python, FastAPI, AsyncIO, REST, WebSockets, SSE</td></tr>
<tr><td><b>Databases</b></td><td>PostgreSQL, MySQL, SQLite, Redis, pgvector</td></tr>
<tr><td><b>Machine Learning</b></td><td>Scikit-Learn, XGBoost, Pandas, NumPy</td></tr>
<tr><td><b>Infrastructure</b></td><td>Docker, Docker Compose, GitHub Actions</td></tr>
<tr><td><b>Applications</b></td><td>Flutter, React Native, ReactJS</td></tr>
<tr><td><b>Engineering Practice</b></td><td>Git, Linux, Automated Testing, CI/CD, API Design</td></tr>
</table>

<br>

## Current Engineering Direction

My primary focus is **production-grade AI engineering** — building systems where AI is one
component of a larger, reliable architecture, rather than an LLM call being the entire application.

<div align="center">

`LLMs` → `RAG / Agents` → `Tool Calling` → `FastAPI Services` → `Databases & Caches` → `Docker + CI/CD` → `Production Applications`

</div>

<br>

## Currently Focused On

<table>
<tr><td width="33%" align="center">🧩<br/><b>Agentic AI Systems</b><br/><sub>LangGraph agents, tool calling, structured outputs</sub></td>
<td width="33%" align="center">🔍<br/><b>RAG & LLM Reliability</b><br/><sub>Retrieval quality, evaluation pipelines, guardrails</sub></td>
<td width="33%" align="center">⚙️<br/><b>Scalable Backend Systems</b><br/><sub>FastAPI, async services, databases, production infra</sub></td></tr>
</table>

<br>

<div align="center">

> Good AI engineering isn't about the model call — it's the backend architecture, data layer, and guardrails that make it reliable in production.

<br>

### Open to opportunities in AI Engineering & Backend Engineering

<br>

[![GitHub](https://img.shields.io/badge/GitHub-jayant132-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/jayant132)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jayantbhatiaa)
[![Email](https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jayantbhatia44@gmail.com)

</div>
