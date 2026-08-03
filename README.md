<div align="center">

```
     ██╗ █████╗ ██╗   ██╗ █████╗ ███╗   ██╗████████╗    ██████╗ ██╗  ██╗ █████╗ ████████╗██╗ █████╗ 
     ██║██╔══██╗╚██╗ ██╔╝██╔══██╗████╗  ██║╚══██╔══╝    ██╔══██╗██║  ██║██╔══██╗╚══██╔══╝██║██╔══██╗
     ██║███████║ ╚████╔╝ ███████║██╔██╗ ██║   ██║       ██████╔╝███████║███████║   ██║   ██║███████║
██   ██║██╔══██║  ╚██╔╝  ██╔══██║██║╚██╗██║   ██║       ██╔══██╗██╔══██║██╔══██║   ██║   ██║██╔══██║
╚█████╔╝██║  ██║   ██║   ██║  ██║██║ ╚████║   ██║       ██████╔╝██║  ██║██║  ██║   ██║   ██║██║  ██║
 ╚════╝ ╚═╝  ╚═╝   ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═══╝   ╚═╝       ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝   ╚═╝   ╚═╝╚═╝  ╚═╝
```

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=17&duration=2800&pause=1200&color=39FF14&center=true&vCenter=true&width=680&lines=AI+Engineer+%7C+RAG+Pipelines+%2B+Autonomous+Agents;booting+production-grade+LLM+systems...;deploying+across+AWS+%2F+Azure+%2F+GCP...;ex-Flutter+dev+%7C+still+obsessed+with+what+breaks;status%3A+open_to_work+%3D%3D+true;" />

**`github.com/jayant132`**

<a href="https://github.com/jayant132"><img src="https://img.shields.io/badge/@jayant132-000000?style=for-the-badge&logo=github&logoColor=39FF14" /></a>
<a href="https://www.linkedin.com/in/jayantbhatiaa"><img src="https://img.shields.io/badge/-LINKEDIN-000000?style=for-the-badge&logo=linkedin&logoColor=39FF14" /></a>
<a href="mailto:jayantbhatia44@gmail.com"><img src="https://img.shields.io/badge/-EMAIL-000000?style=for-the-badge&logo=gmail&logoColor=39FF14" /></a>

<img src="https://komarev.com/ghpvc/?username=jayant132&label=PROFILE+VIEWS&color=39FF14&style=for-the-badge&labelColor=000000" />

</div>

<br/>

```
[  OK  ] Loading jayant_bhatia.profile
[  OK  ] Mounting /projects
[  OK  ] Initializing AI_ENGINEER module
[  OK  ] Linking LangChain :: RAG :: Google ADK :: Agents
[  OK  ] Connecting cloud/aws-ec2 ................ UP
[  OK  ] Connecting cloud/azure-data-factory ..... UP
[  OK  ] Verifying production-readiness ......... PASS
[ INFO ] Legacy module detected: flutter_dev.so (still loaded, not deprecated)
[ READY ] system online. awaiting query_
```

<br/>

<div align="center">

### `$ neofetch`

</div>

```
              ▄▄▄▄▄▄▄▄▄▄▄                    jayant@ai-engineer  ~  @jayant132
           ▄██▀▀▀▀▀▀▀▀▀██▄                   ────────────────────────────────
          ██▀   ▄▄▄▄▄   ▀██                  OS: Production Systems v2
         ██   ▄█▀▀▀▀▀█▄   ██                 Role: AI Engineer
        ██   ██   █   ██   ██                Shell: /bin/python3 + LangChain
        ██   ██  ███  ██   ██                Agent Framework: Google ADK
        ██   ▀█▄▄▄▄▄█▀   ██                  Cloud: AWS EC2 · Azure Data Factory
         ██▄   ▀▀▀▀▀   ▄██                   Background: Flutter / Dart (mobile)
          ▀██▄▄▄▄▄▄▄▄▄██▀                    Philosophy: ship > demo
             ▀▀▀▀▀▀▀▀▀                       Status: open_to_work → true
```

<br/>

> **⚡ recruiter_summary.txt** — I build production-grade RAG pipelines and autonomous LLM agents, not notebook demos — deployed on real cloud infrastructure, not just `localhost`. My Flutter background means I already know what "works for real users" costs, and I bring that standard to every model, pipeline, and agent I ship.

<br/>

<div align="center">

### `$ ./agent_demo.sh --trace`

*a peek at how the agent actually thinks, not just what it outputs*

</div>

```
› user     : "What changed in our refund policy this quarter?"

› agent    : plan → needs current source-of-truth, not memory
           ↳ tool_call: hybrid_retrieve(query="refund policy Q3 changes")
           ↳ tool_call: rerank(top_k=25 → top_k=5)
           ↳ checking: are results grounded above confidence threshold?
           ↳ result   : YES (4/5 chunks agree, 1 outlier discarded)

› agent    : "Refund window extended 14 → 30 days, effective Q3.
              Source: policy_v4.pdf, §2.1 [confidence: high]"

› agent    : if confidence had been LOW →
           ↳ fallback: "I don't have a grounded answer — escalating
              to clarification instead of guessing."
```


<br/>

<div align="center">

### `$ cat architecture/*.log`

</div>

**RAG Pipeline — engineered to be *wrong less often*, not just fast**

```
 User Query
     │
     ▼
 Query Understanding
     │
     ▼
 Hybrid Retrieval ────────► Vector Store
     │                            │
     ▼                            ▼
 Re-ranking ◄────────────────────┘
     │
     ▼
 Context Assembly
     │
     ▼
 LLM Generation
     │
     ▼
 Grounded in source? ──Yes──► Answer + Citations
     │
     No
     ▼
 Fallback / Clarify   ◄── I'd rather say "I don't know" than hallucinate
```

**Agent Reasoning Loop — plans before it acts (Google ADK)**

```
 Goal Received
     │
     ▼
┌──► Plan Next Step
│         │
│         ▼
│    Select Tool ──► Execute Action
│                          │
│                          ▼
│                   Goal Complete?
│                     │        │
└─────────No──────────┘       Yes
                                │
                                ▼
                         Return Result
```

**Deployment Path — code to cloud**

```
 Local Dev
     │
     ▼
 Containerize
     │
     ▼
 AWS EC2 ──────► Serving Layer (agent / RAG API)
     │
     ▼
 Azure Data Factory ──► ETL / pipeline scheduling
     │                       for retrieval-source freshness
     ▼
 Monitoring & Fallback Logs
```


<br/>

<div align="center">

### `$ ls -la ~/projects/`

</div>

```
drwxr-xr-x  jayant132  rag-chatbot/
```
**Intelligent Chatbot (RAG)** — Retrieval-grounded Q&A over a custom knowledge base, built to minimize hallucination rather than just demo well on easy queries.
`> problem:` generic LLMs don't know your org's data, and naive RAG returns confident nonsense.
`LangChain` `LLMs` `Vector Retrieval` `Prompt Engineering` · [`git clone →`](https://github.com/jayant132)

```
drwxr-xr-x  jayant132  agent-automation/
```
**AI Agent Automation System** — An autonomous agent (built on Google ADK) that plans across multiple steps, selects tools, and executes workflows with minimal human input.
`> problem:` most "AI automation" is one prompt in a trench coat. This reasons about what to do next, not just what to say next.
`Google ADK` `AI Agents` `Tool Use` `LLM Orchestration` `APIs` · [`git clone →`](https://github.com/jayant132)

<sub>💡 swap in your real repo URLs once pushed</sub>

<br/>

<div align="center">

### `$ cat /proc/stack`

<img src="https://skillicons.dev/icons?i=python,langchain,aws,azure,gcp,flutter,dart,git,github,postgres&theme=dark" />

</div>

<br/>

```
┌─ stack.json ──────────────────────────────────────────────────────┐
│  AI Engineering    │ LLMs · LangChain · Google ADK · RAG ·         │
│                     │ Prompt Engineering · AI Agents                │
│  Backend & APIs    │ Python · REST APIs · Microservices             │
│  Cloud & Infra      │ Amazon EC2 · Azure Data Factory · Docker      │
│  Data & Query      │ SQL · Pandas · NumPy                           │
│  Also fluent in    │ Flutter · Dart                                 │
└──────────────────────────────────────────────────────────────────┘
```

<br/>

<div align="center">

### `$ cat principles.md`

</div>

```
┌─ principle ──────────────────────┬─ in practice ──────────────────────────────┐
│ ship over demo                   │ works on 3 curated questions ≠ done.        │
│                                   │ that's a prototype.                         │
│ traceable AI                     │ if it can't explain why it answered,        │
│                                   │ I don't trust it in prod.                   │
│ engineering first                │ latency, cost, failure modes matter as      │
│                                   │ much as model choice.                       │
│ narrow & reliable > broad & flaky│ one thing that always works beats five      │
│                                   │ that sometimes do.                          │
└───────────────────────────────────┴─────────────────────────────────────────────┘
```

<br/>

<details>
<summary><code>$ cat currently_exploring.txt</code></summary>
<br/>

```
> hybrid retrieval         — dense + sparse search for better recall
> agent evaluation         — past "worked once" toward measurable reliability
> multi-agent coordination — where one agent's context window bottlenecks
> cost-aware architecture  — same quality, lower latency and spend on EC2
> pipeline scheduling      — Azure Data Factory for retrieval-source freshness
```

</details>

<br/>

<div align="center">

### `$ ./skill_matrix.sh --verbose`

</div>

```
┌─ proficiency.log ──────────────────────────────────────────────┐
│                                                                  │
│  LangChain / RAG Systems   ███████████████████░░░  85%          │
│  LLM Agents (Google ADK)   ████████████████░░░░░░  75%          │
│  Python                    ████████████████████░░  90%          │
│  Prompt Engineering        ██████████████████░░░░  82%          │
│  Cloud (AWS EC2 / Azure)   ███████████████░░░░░░░  70%          │
│  Flutter / Dart            ███████████████████░░░  85%          │
│  SQL / Data Pipelines      ████████████████░░░░░░  75%          │
│                                                                  │
└──────────────────────────────────────────────────────────────────┘
```


<br/>

<div align="center">

### `$ git log --oneline --graph career.timeline`

</div>

```
*  2026 ── status: hardening evaluation, targeting AI Engineer roles
│
*  2025 ── shipped agent-automation → multi-step autonomous agent (Google ADK)
│
*  2025 ── shipped rag-chatbot → hybrid retrieval + re-ranking + citations
│
*  2024 ── pip install langchain → began the shift into AI engineering
│
*  2023 ── flutter build --release → shipped production mobile apps
│         (learned: every crash is your problem, in prod, not a notebook)
```


<br/>

<div align="center">

```
┌──────────────────────────────────────────────────────────┐
│ jayant@terminal:~$ echo "let's build something"           │
│ > open to AI Engineer roles — end-to-end ownership,       │
│   not just prompt-tuning.                                 │
│ jayant@terminal:~$ _                                       │
└──────────────────────────────────────────────────────────┘
```

<a href="https://github.com/jayant132"><img src="https://img.shields.io/badge/@jayant132-000000?style=for-the-badge&logo=github&logoColor=39FF14" /></a>
<a href="https://www.linkedin.com/in/jayantbhatiaa"><img src="https://img.shields.io/badge/CONNECT_ON_LINKEDIN-000000?style=for-the-badge&logo=linkedin&logoColor=39FF14" /></a>
<a href="mailto:jayantbhatia44@gmail.com"><img src="https://img.shields.io/badge/EMAIL_ME-000000?style=for-the-badge&logo=gmail&logoColor=39FF14" /></a>

<br/>


</div>
