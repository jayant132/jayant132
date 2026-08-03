<div align="center">

# JAYANT BHATIA

### AI Engineer — systems that reason, retrieve & act

[![LinkedIn](https://img.shields.io/badge/LINKEDIN-000000?style=flat-square&logo=linkedin&logoColor=39FF14&labelColor=000000)](https://www.linkedin.com/in/jayantbhatiaa)
[![Email](https://img.shields.io/badge/EMAIL-000000?style=flat-square&logo=gmail&logoColor=39FF14&labelColor=000000)](mailto:jayantbhatia44@gmail.com)
[![GitHub](https://img.shields.io/badge/GITHUB-000000?style=flat-square&logo=github&logoColor=39FF14&labelColor=000000)](https://github.com/jayant132)

</div>

<br/>

```
┌──────────────────────────────────────────────────────┐
│ jayant@terminal:~$ whoami                              │
│ AI Engineer building LLM systems that work in          │
│ production — not just in a notebook.                   │
└──────────────────────────────────────────────────────┘
```

<br/>

## `$ cat about.txt`

I build retrieval-grounded and agentic LLM systems — RAG pipelines that cite their sources, and agents that reason about what to do next instead of just what to say next.

Before AI, I shipped production Flutter apps, where every crash and every millisecond of jank was my problem live, not in a notebook. That standard — latency, failure modes, and things actually working under real users — is the one I hold every pipeline and agent to.

<br/>

## `$ cat pipeline.log`

**RAG Pipeline**

```
 User Query
     |
     v
 Query Understanding
     |
     v
 Hybrid Retrieval ----> Vector Store
     |                       |
     v                       v
 Re-ranking <----------------+
     |
     v
 Context Assembly
     |
     v
 LLM Generation
     |
     v
 Grounded in source? --Yes--> Answer + Citations
     |
     No
     v
 Fallback / Clarify
```

**Agent Reasoning Loop**

```
 Goal Received
     |
     v
+--> Plan Next Step
|         |
|         v
|    Select Tool --> Execute Action
|                          |
|                          v
|                   Goal Complete?
|                     |        |
+---------No----------+       Yes
                                |
                                v
                         Return Result
```

> Design choices, not defaults: re-ranking exists because naive top-k retrieval was returning plausible-but-wrong context. The fallback branch exists because I'd rather the system say "I don't know" than hallucinate.

<br/>

## `$ ls projects/`

**`rag-chatbot/`** — Intelligent Chatbot (RAG)
Retrieval-grounded Q&A over a custom knowledge base, built to minimize hallucination rather than just demo well on easy queries.
Problem it solves: generic LLMs don't know your org's data, and naive RAG returns confident nonsense.
`LangChain` `LLMs` `Vector Retrieval` `Prompt Engineering`

**`agent-automation/`** — AI Agent Automation System
An autonomous agent that plans across multiple steps, selects tools, and executes workflows with minimal human input.
Problem it solves: most "AI automation" is one prompt in a trench coat. This reasons about what to do next, not just what to say next.
`AI Agents` `Tool Use` `LLM Orchestration` `APIs`

<br/>

## `$ cat stack.json`

| Domain | Tools |
|---|---|
| AI Engineering | LLMs · LangChain · RAG · Prompt Engineering · AI Agents |
| Backend & APIs | Python · REST APIs |
| Data & Query | SQL · Pandas · NumPy |
| Also fluent in | Flutter · Dart |
| Tooling | Git · GitHub |

<br/>

## `$ cat principles.md`

| Principle | In practice |
|---|---|
| Ship over demo | A pipeline that works on 3 curated questions isn't done — it's a prototype. |
| Traceable AI | If a system can't explain why it answered something, I don't trust it in production. |
| Engineering first | Latency, cost, and failure modes matter as much as model choice. |
| Narrow and reliable > broad and flaky | I'd rather ship an agent that reliably does one thing than one that sometimes does five. |

<br/>

<details>
<summary><code>$ cat currently_exploring.txt</code></summary>
<br/>

- Hybrid retrieval — combining dense + sparse search for better recall on ambiguous queries
- Agent evaluation — moving past "it worked in my test run" toward measurable reliability
- Multi-agent coordination — where a single agent's context window becomes the bottleneck
- Cost-aware LLM architecture — same output quality, lower latency and spend

</details>

<br/>

## `$ fetch --stats`

<div align="center">

![stats](https://github-readme-stats.vercel.app/api?username=jayant132&show_icons=true&theme=dark&hide_border=true&bg_color=000000&title_color=39FF14&icon_color=39FF14&text_color=39FF14)
![streak](https://github-readme-streak-stats.herokuapp.com/?user=jayant132&theme=dark&hide_border=true&background=000000&ring=39FF14&fire=39FF14&currStreakLabel=39FF14)

</div>

<br/>

<div align="center">

```
┌──────────────────────────────────────────────────────┐
│ jayant@terminal:~$ echo "let's talk"                   │
│ Open to AI Engineer roles — end-to-end ownership,       │
│ not just prompt-tuning.                                 │
└──────────────────────────────────────────────────────┘
```

[![LinkedIn](https://img.shields.io/badge/CONNECT_ON_LINKEDIN-000000?style=for-the-badge&logo=linkedin&logoColor=39FF14&labelColor=000000)](https://www.linkedin.com/in/jayantbhatiaa)
[![Email](https://img.shields.io/badge/EMAIL_ME-000000?style=for-the-badge&logo=gmail&logoColor=39FF14&labelColor=000000)](mailto:jayantbhatia44@gmail.com)

</div>
