<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,100:14B8A6&height=190&section=header&text=JAYANT%20BHATIA&fontSize=50&fontColor=ffffff&fontAlignY=38&desc=AI%20Systems%20%26%20Backend%20Engineer&descAlignY=58&descSize=18&animation=fadeIn" width="100%"/>

<a href="https://github.com/jayant132"><img src="https://img.shields.io/badge/GitHub-jayant132-0F172A?style=for-the-badge&logo=github&logoColor=14B8A6" alt="GitHub"></a>
<a href="https://www.linkedin.com/in/jayantbhatiaa"><img src="https://img.shields.io/badge/LinkedIn-Connect-0F172A?style=for-the-badge&logo=linkedin&logoColor=14B8A6" alt="LinkedIn"></a>
<a href="mailto:jayantbhatia44@gmail.com"><img src="https://img.shields.io/badge/Email-Reach_Out-0F172A?style=for-the-badge&logo=gmail&logoColor=14B8A6" alt="Email"></a>

<br><br>

<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&weight=500&size=19&duration=2800&pause=900&color=14B8A6&center=true&vCenter=true&width=680&lines=Generative+AI+%2B+Agentic+Systems;RAG+pipelines+that+don't+hallucinate+silently;Natural+language+%E2%86%92+SQL+%E2%86%92+action;Red-teaming+the+agents+I+build+before+you+do" alt="Typing SVG" />

<br>

`AI ENGINEER`  ·  `AGENTIC SYSTEMS`  ·  `BACKEND`  ·  `AI SECURITY`

</div>

<br>

## `whoami`

I build the layer between an LLM and something people can actually rely on — retrieval that's grounded, agents that fail safely, and backend systems that hold up when a model call is slow, wrong, or actively attacked.

The model call is the easy part. The interesting engineering is everywhere around it.

<table>
<tr>
<td width="58%" valign="top">

```python
class JayantBhatia:
    focus      = ["Agentic AI", "RAG", "Backend Systems", "AI Security"]
    stack      = ["Python", "FastAPI", "LangGraph", "PostgreSQL"]
    background = "Software Engineering → AI Engineering"

    def philosophy(self) -> str:
        return (
            "An agent is only as trustworthy as its worst-case "
            "behavior under adversarial input — I test for that "
            "before I ship anything."
        )
```

</td>
<td width="42%" valign="top">

**Right now:**
- 🔴 Red-teaming my own agents before anyone else does
- 🗣️ Natural language → SQL → real database actions
- 🧩 Multi-agent orchestration with LangGraph
- 🗄️ RAG grounded in pgvector, not vibes

</td>
</tr>
</table>

<br>

## Flagship builds

Every project here ships a number, not an adjective. If a claim can't be measured, it isn't in this section.

<table>
<tr>
<td width="50%" valign="top">

### 🛡️ Agentic Red Team Framework
*What happens when someone actively tries to break a tool-using agent?*

Attacks agents across 4 tool surfaces — web search, filesystem, database, external API — with 7 attack classes: prompt injection, privilege escalation, data exfiltration, excessive agency. Scored on a 4-level rubric, not pass/fail.

|  | Undefended | Defended |
|---|:---:|:---:|
| Mock backend | 0 / 7 | **6 / 7** |
| Ollama (llama3.2:1b) | 6 / 7 | **7 / 7** |

CI-gated at an 85% defended-pass threshold. Mapped to OWASP's Agentic AI threat taxonomy.

`Python` `ReAct loop` `Ollama` `pytest` `GitHub Actions`

**[→ View repo](https://github.com/jayant132/Agentic-Red-Team-Framework)**

</td>
<td width="50%" valign="top">

### 🔐 MCP Guardrail
*Most agent red-teaming skips the tool catalog — this attacks it directly.*

Targets the MCP trust boundary: tool-description poisoning, indirect injection via tool output, credential exposure, allowlist bypass. Same rubric discipline as the framework above.

|  | Undefended | Defended |
|---|:---:|:---:|
| Mock backend | 0 / 5 | **5 / 5** |
| Ollama (llama3.2:1b) | 5 / 5 | **5 / 5** |

One honest finding: a sanitizer gap (paraphrase evasion) slipped past the first defense layer, caught only by an independent allowlist check — the kind of failure most portfolios quietly omit.

`Python` `MCP Protocol` `Ollama` `pytest`

**[→ View repo](https://github.com/jayant132/MCP-Guardrail)**

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🗣️ SQL AGENT LLM
*Natural language in. A safe, executed query out.*

An LLM agent that translates plain-English questions into SQL, executes them, and returns results — the same tool-calling discipline as the red-team projects above, applied to a real, everyday agentic use case rather than a synthetic benchmark.

`LLM tool calling` `SQL generation` `Python`

**[→ View repo](https://github.com/jayant132/Sql_Agent_llm)**

</td>
<td width="50%" valign="top">

### ✈️ Multi-Agent Flight Booking Assistant
An orchestrator delegates across **search, booking, and support agents**, each scoped to its own tools — instead of one model trying to hold the entire workflow in a single context window.

```
        USER
         │
   ORCHESTRATOR
   ╱     │     ╲
SEARCH BOOKING SUPPORT
   ╲     │     ╱
     TOOLS → RESULT
```

`Multi-agent orchestration` `Tool calling` `Python`

**[→ View repo](https://github.com/jayant132/Multi-Agent-AI-Flight-Booking-Assistant-)**

</td>
</tr>
</table>

<br>

## Also shipped

<table>
<tr>
<td width="33%" valign="top">

**🧾 Invoice Intelligence**

Two ML pipelines on real procurement data. Engineering a single feature — the invoice/PO dollar gap — took flagged-invoice recall from **17% → 99%** on the same dataset.

`Scikit-learn` `Pandas` `SQLite`

**[→ View repo](https://github.com/jayant132/Invoice-Intelligence-ML-Project)**

</td>
<td width="33%" valign="top">

**🫁 Tuberculosis Detection ML**

Chest X-ray classification with a structured pipeline — separate `src`, `experiments`, and `docs` — rather than a single notebook.

`Computer Vision` `Model Evaluation`

**[→ View repo](https://github.com/jayant132/Tuberculosis-Detection-ML)**

</td>
<td width="33%" valign="top">

**📊 JPMorgan Forage — Quant Research**

Completed JPMorgan Chase's official Forage quantitative-research job simulation.

`Applied Quant Research`

**[→ View repo](https://github.com/jayant132/-JP-Morgan-Quantitative-Research-Virtual-Internship)**

</td>
</tr>
</table>

<br>

## How the layers fit together

<div align="center">

| Layer | What lives here |
|---|---|
| **Application** | Flutter · React Native · Web clients |
| **Backend** | FastAPI · AsyncIO · REST / WebSocket · Auth & validation |
| **AI / Agents** | LLMs · RAG · LangGraph orchestration · Tool calling |
| **Data** | PostgreSQL · pgvector · Redis · SQLite |

</div>

**The rule I hold to:** business rules and validation stay in deterministic code. The LLM is called only where reasoning or language generation is doing work no `if` statement could — not because routing everything through a model is fashionable.

<br>

## Stack

<table>
<tr><th align="left" width="20%">Domain</th><th align="left">Tools</th></tr>
<tr><td><b>AI / Agentic</b></td><td>LangGraph · LangChain · Google ADK · RAG · Tool calling · Prompt engineering</td></tr>
<tr><td><b>AI Security</b></td><td>Prompt-injection defense · agent red-teaming · MCP trust-boundary testing · OWASP GenAI mapping</td></tr>
<tr><td><b>Backend</b></td><td>Python · FastAPI · AsyncIO · REST · WebSockets · SSE</td></tr>
<tr><td><b>Data</b></td><td>PostgreSQL · pgvector · Redis · MySQL · SQLite</td></tr>
<tr><td><b>ML</b></td><td>Scikit-learn · XGBoost · Pandas · NumPy</td></tr>
<tr><td><b>Infra</b></td><td>Docker · Docker Compose · GitHub Actions</td></tr>
<tr><td><b>Apps</b></td><td>Flutter · React Native · React</td></tr>
</table>

<br>

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=jayant132&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0F172A&title_color=14B8A6&icon_color=14B8A6&text_color=E2E8F0" height="165"/>
<img src="https://github-readme-streak-stats.herokuapp.com/?user=jayant132&theme=tokyonight&hide_border=true&background=0F172A&ring=14B8A6&fire=14B8A6&currStreakLabel=14B8A6" height="165"/>

</div>

<br>

<div align="center">

### Open to AI Engineering & Backend Engineering roles — remote-friendly, open to relocation

<a href="https://github.com/jayant132"><img src="https://img.shields.io/badge/GitHub-jayant132-0F172A?style=for-the-badge&logo=github&logoColor=14B8A6"></a>
<a href="https://www.linkedin.com/in/jayantbhatiaa"><img src="https://img.shields.io/badge/LinkedIn-Connect-0F172A?style=for-the-badge&logo=linkedin&logoColor=14B8A6"></a>
<a href="mailto:jayantbhatia44@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-0F172A?style=for-the-badge&logo=gmail&logoColor=14B8A6"></a>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:14B8A6,100:0F172A&height=100&section=footer" width="100%"/>

</div>
