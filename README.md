<div align="center">

# Jayant Bhatia

### AI Systems & Backend Engineer

**Agentic AI · RAG · Python · FastAPI · AI Security**

<br>

<a href="https://github.com/jayant132"><img src="https://img.shields.io/badge/GitHub-jayant132-2b2b2b?style=for-the-badge&logo=github&logoColor=14B8A6" /></a>
<a href="https://www.linkedin.com/in/jayantbhatiaa"><img src="https://img.shields.io/badge/LinkedIn-Connect-2b2b2b?style=for-the-badge&logo=linkedin&logoColor=14B8A6" /></a>
<a href="mailto:jayantbhatia44@gmail.com"><img src="https://img.shields.io/badge/Email-Reach_Out-2b2b2b?style=for-the-badge&logo=gmail&logoColor=14B8A6" /></a>

</div>

<br>

<div align="center">

*I build the layer between an LLM and something people can actually rely on — retrieval that's grounded, agents that fail safely, and backend systems that hold up under load and under attack.*

**The model call is the easy part. The engineering happens everywhere around it.**

</div>

<br>

<div align="center">

<img src="https://skillicons.dev/icons?i=python,fastapi,postgres,redis,docker,githubactions,flutter,react,git&theme=dark" />

</div>

<br><br>

## 🛡️ Flagship Builds

*Every project below reports a number, not an adjective.*

<br>

### Agentic Red Team Framework
What happens when someone actively tries to break a tool-using agent? Attacks agents across 4 tool surfaces — web search, filesystem, database, external API — with 7 attack classes: prompt injection, privilege escalation, data exfiltration, excessive agency. Scored on a 4-level outcome rubric, not pass/fail, and CI-gated at an 85% defended-pass threshold.

| Backend | Undefended | Defended |
|:--|:--:|:--:|
| Mock | 0 / 7 | **6 / 7** ✅ |
| Ollama (llama3.2:1b) | 6 / 7 | **7 / 7** ✅ |

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/> <img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white"/> <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/> <img src="https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white"/>

**→ [View repository](https://github.com/jayant132/Agentic-Red-Team-Framework)**

<br>

### MCP Guardrail
Most agent red-teaming skips the tool catalog itself — this attacks it directly. Targets the MCP trust boundary: tool-description poisoning, indirect injection via tool output, credential exposure, allowlist bypass.

| Backend | Undefended | Defended |
|:--|:--:|:--:|
| Mock | 0 / 5 | **5 / 5** ✅ |
| Ollama (llama3.2:1b) | 5 / 5 | **5 / 5** ✅ |

> ⚠️ **Documented finding:** a sanitizer gap (paraphrase evasion) slipped past the first defense layer, caught only by an independent allowlist check — logged honestly rather than hidden, because that's the failure mode that actually matters.

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/> <img src="https://img.shields.io/badge/MCP_Protocol-6E56CF?style=flat-square"/> <img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white"/>

**→ [View repository](https://github.com/jayant132/MCP-Guardrail)**

<br>

### SQL AGENT LLM
Natural language in, a safe executed query out. Translates plain-English questions into SQL, executes them, and returns results — the same tool-calling discipline as the projects above, applied to a real everyday agentic workflow instead of a synthetic benchmark.

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/> <img src="https://img.shields.io/badge/LLM_Tool_Calling-14B8A6?style=flat-square"/> <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white"/>

**→ [View repository](https://github.com/jayant132/Sql_Agent_llm)**

<br>

### Multi-Agent Flight Booking Assistant
One orchestrator delegates to three scoped agents — search, booking, support — instead of forcing a single model to hold the entire workflow in one context window.

| Agent | Scope |
|:--|:--|
| `SEARCH_AGENT` | Flight lookup tools |
| `BOOKING_AGENT` | Reservation tools |
| `SUPPORT_AGENT` | Post-booking tools |

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/> <img src="https://img.shields.io/badge/Multi--Agent_Orchestration-14B8A6?style=flat-square"/> <img src="https://img.shields.io/badge/Tool_Calling-14B8A6?style=flat-square"/>

**→ [View repository](https://github.com/jayant132/Multi-Agent-AI-Flight-Booking-Assistant-)**

<br><br>

## 📦 Also Shipped

| Project | What it does | Stack |
|:--|:--|:--|
| **[Invoice Intelligence](https://github.com/jayant132/Invoice-Intelligence-ML-Project)** | One engineered feature — the invoice/PO dollar gap — took flagged-invoice recall from **17% → 99%** | Scikit-learn · Pandas · SQLite |
| **[Tuberculosis Detection ML](https://github.com/jayant132/Tuberculosis-Detection-ML)** | Chest X-ray classification with a real pipeline structure — separate `src`, `experiments`, `docs` | Computer Vision · Model Evaluation |
| **[JPMorgan Forage — Quant Research](https://github.com/jayant132/-JP-Morgan-Quantitative-Research-Virtual-Internship)** | Completed JPMorgan Chase's official Forage quant-research job simulation | Applied Quant Research |

<br><br>

## 🧱 System Architecture

| Layer | Tech |
|:--|:--|
| **Application** | Flutter · React Native · Web |
| **Backend** | FastAPI · AsyncIO · REST / WebSocket |
| **AI / Agents** | LLMs · RAG · LangGraph · Tool Calling |
| **Data** | PostgreSQL · pgvector · Redis · SQLite |

**The rule I hold to:** business logic stays deterministic. The LLM only runs where reasoning or generation is doing work an `if` statement can't.

<br><br>

## ⚙️ Stack

| Domain | Tools |
|:--|:--|
| **AI / Agentic** | LangGraph · LangChain · Google ADK · RAG · Tool Calling · Prompt Engineering |
| **AI Security** | Prompt-injection defense · Agent red-teaming · MCP trust-boundary testing · OWASP GenAI mapping |
| **Backend** | Python · FastAPI · AsyncIO · REST · WebSockets · SSE |
| **Data** | PostgreSQL · pgvector · Redis · MySQL · SQLite |
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
