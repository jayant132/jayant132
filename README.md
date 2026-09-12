<div align="center">

```
╔═══════════════════════════════════════════════════════════╗
║  SYSTEM BOOT — v2.6                                        ║
╠═══════════════════════════════════════════════════════════╣
║                                                             ║
║  > initializing profile..................... [ OK ]        ║
║  > loading identity.......................... [ OK ]        ║
║  > mounting stack............................ [ OK ]        ║
║  > running self-diagnostics.................. [ OK ]        ║
║                                                             ║
║  ───────────────────────────────────────────────────────  ║
║  NAME     : JAYANT BHATIA                                  ║
║  ROLE     : AI Systems & Backend Engineer                  ║
║  FOCUS    : Agentic AI · RAG · Python · FastAPI · Security ║
║  STATUS   : ONLINE                                         ║
║  ───────────────────────────────────────────────────────  ║
║                                                             ║
║  [READY]                                                   ║
║                                                             ║
╚═══════════════════════════════════════════════════════════╝
```

**[GitHub](https://github.com/jayant132) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/jayantbhatiaa) &nbsp;·&nbsp; [Email](mailto:jayantbhatia44@gmail.com)**

</div>

<br>

```
> loading manifesto.md.................. [ OK ]
```

> I build the layer between an LLM and something people can actually rely on —
> retrieval that's grounded, agents that fail safely, and backend systems that
> hold up when a model call is slow, wrong, or actively attacked.
>
> The model call is the easy part. The interesting engineering happens everywhere
> around it — and I test my own agents adversarially before anyone else does.

<br>

```
> reading config.yaml................... [ OK ]
```

```yaml
role:        AI Systems & Backend Engineer
background:  Software Engineering → AI Engineering
stack:       [Python, FastAPI, LangGraph, PostgreSQL, pgvector, Docker]
principle:   business logic stays deterministic — the LLM only runs where
             reasoning or generation does work an if-statement can't
status:      open to AI Engineering & Backend Engineering roles
             remote-friendly · open to relocation
```

<br>

## `> mounting /flagship-builds ........... [ OK ]`

Every project below reports a number, not an adjective. No measurement, no mention.

<br>

```
> booting module: agentic-red-team-framework .......... [ OK ]
```

**🛡️ Agentic Red Team Framework** — *what happens when someone actively tries to break a tool-using agent?*

Attacks agents across 4 tool surfaces (web search, filesystem, database, external API) with 7 attack classes — prompt injection, privilege escalation, data exfiltration, excessive agency. Scored on a 4-level outcome rubric, not pass/fail. CI-gated at an 85% defended-pass threshold. Mapped to OWASP's Agentic AI threat taxonomy.

```
[BENCHMARK RESULTS]
  backend                undefended    defended
  ─────────────────────────────────────────────
  mock                      0/7        6/7  [PASS]
  ollama (llama3.2:1b)      6/7        7/7  [PASS]
```

`Python` `ReAct loop` `Ollama` `pytest` `GitHub Actions` → **[view repo](https://github.com/jayant132/Agentic-Red-Team-Framework)**

<br>

```
> booting module: mcp-guardrail ........................ [ OK ]
```

**🔐 MCP Guardrail** — *most agent red-teaming skips the tool catalog itself. this attacks it directly.*

Targets the MCP trust boundary: tool-description poisoning, indirect injection via tool output, credential exposure, allowlist bypass. Same rubric discipline as the framework above.

```
[BENCHMARK RESULTS]
  backend                undefended    defended
  ─────────────────────────────────────────────
  mock                      0/5        5/5  [PASS]
  ollama (llama3.2:1b)      5/5        5/5  [PASS]

[WARNING LOG]
  sanitizer gap detected: paraphrase evasion slipped past the first
  defense layer — caught only by an independent allowlist check.
  logged honestly instead of hidden, because that's the failure
  mode that actually matters.
```

`Python` `MCP Protocol` `Ollama` `pytest` → **[view repo](https://github.com/jayant132/MCP-Guardrail)**

<br>

```
> booting module: sql-agent-llm ......................... [ OK ]
```

**🗣️ SQL AGENT LLM** — *natural language in. a safe, executed query out.*

An LLM agent that translates plain-English questions into SQL, executes them, and returns results — the same tool-calling discipline as the projects above, applied to a real everyday agentic workflow instead of a synthetic benchmark.

`LLM tool calling` `SQL generation` `Python` → **[view repo](https://github.com/jayant132/Sql_Agent_llm)**

<br>

```
> booting module: flight-booking-assistant .............. [ OK ]
```

**✈️ Multi-Agent Flight Booking Assistant**

```
[PROCESS TREE]
ORCHESTRATOR
   ├── SEARCH_AGENT   → flight lookup tools
   ├── BOOKING_AGENT  → reservation tools
   └── SUPPORT_AGENT  → post-booking tools
```

One orchestrator delegates to three scoped agents instead of forcing a single model to hold the entire workflow in one context window.

`Multi-agent orchestration` `Tool calling` `Python` → **[view repo](https://github.com/jayant132/Multi-Agent-AI-Flight-Booking-Assistant-)**

<br>

## `> mounting /also-shipped ............... [ OK ]`

<table>
<tr>
<td width="33%" valign="top">

**🧾 Invoice Intelligence**

One engineered feature — the invoice/PO dollar gap — took flagged-invoice recall from **17% → 99%** on the same dataset.

`Scikit-learn` `Pandas`
**[→ repo](https://github.com/jayant132/Invoice-Intelligence-ML-Project)**

</td>
<td width="33%" valign="top">

**🫁 Tuberculosis Detection**

Chest X-ray classification with a real pipeline structure — separate `src`, `experiments`, `docs`.

`Computer Vision`
**[→ repo](https://github.com/jayant132/Tuberculosis-Detection-ML)**

</td>
<td width="33%" valign="top">

**📊 JPMorgan Forage**

Completed JPMorgan Chase's official Forage quant-research job simulation.

`Applied Quant Research`
**[→ repo](https://github.com/jayant132/-JP-Morgan-Quantitative-Research-Virtual-Internship)**

</td>
</tr>
</table>

<br>

## `> reading system_architecture.log ...... [ OK ]`

```
┌───────────────────────────────────────────────┐
│  APPLICATION   Flutter · React Native · Web    │
├───────────────────────────────────────────────┤
│  BACKEND       FastAPI · AsyncIO · REST / WS   │
├───────────────────────────────────────────────┤
│  AI / AGENTS   LLMs · RAG · LangGraph · Tools  │
├───────────────────────────────────────────────┤
│  DATA          PostgreSQL · pgvector · Redis   │
└───────────────────────────────────────────────┘
```

<br>

## `> loading stack.yaml ................... [ OK ]`

```yaml
ai_agentic:    [LangGraph, LangChain, Google ADK, RAG, Tool Calling, Prompt Engineering]
ai_security:   [Prompt-Injection Defense, Agent Red-Teaming, MCP Trust Boundaries, OWASP GenAI]
backend:       [Python, FastAPI, AsyncIO, REST, WebSockets, SSE]
data:          [PostgreSQL, pgvector, Redis, MySQL, SQLite]
ml:            [Scikit-learn, XGBoost, Pandas, NumPy]
infra:         [Docker, Docker Compose, GitHub Actions]
apps:          [Flutter, React Native, React]
```

<br>

```
> running final diagnostics ............. [ OK ]
```

```
[SYSTEM STATUS]
  repositories        : 21
  primary language    : Python
  focus               : agentic systems tested adversarially, not just demoed
  status              : OPEN TO OPPORTUNITIES
  roles               : AI Engineering · Backend Engineering
  availability        : remote-friendly · open to relocation

[END OF LOG]
```

<br>

<div align="center">

```
╔═══════════════════════════════════════════════════════════╗
║  > connection request..................... [ SEND ]        ║
╚═══════════════════════════════════════════════════════════╝
```

**[GitHub](https://github.com/jayant132) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/jayantbhatiaa) &nbsp;·&nbsp; [Email](mailto:jayantbhatia44@gmail.com)**

</div>
