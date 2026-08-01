<div align="center">

![banner](https://capsule-render.vercel.app/api?type=blur&amp;color=0:000000,100:0d1f0d&amp;height=200&amp;section=header&amp;text=JAYANT%20BHATIA&amp;fontSize=42&amp;fontColor=39FF14&amp;desc=AI%20ENGINEER%20//%20systems%20that%20reason,%20retrieve%20%26%20act&amp;descSize=14&amp;descAlignY=68&amp;fontAlignY=38&amp;animation=fadeIn)

![typing](https://readme-typing-svg.demolab.com?font=Courier+New&amp;weight=700&amp;size=18&amp;pause=1800&amp;color=39FF14&amp;center=true&amp;vCenter=true&amp;width=600&amp;lines=%3E+building+LLM+systems+that+survive+production_;%3E+RAG+pipelines+.+AI+agents+.+LangChain_;%3E+ex-mobile+engineer+%7C+now+AI+engineer_)

[![LinkedIn](https://img.shields.io/badge/LINKEDIN-000000?style=flat-square&amp;logo=linkedin&amp;logoColor=39FF14&amp;labelColor=000000)](https://www.linkedin.com/in/jayantbhatiaa)
[![Email](https://img.shields.io/badge/EMAIL-000000?style=flat-square&amp;logo=gmail&amp;logoColor=39FF14&amp;labelColor=000000)](mailto:jayantbhatia44@gmail.com)
[![GitHub](https://img.shields.io/badge/GITHUB-000000?style=flat-square&amp;logo=github&amp;logoColor=39FF14&amp;labelColor=000000)](https://github.com/YOUR_GITHUB_USERNAME)

</div>

<br/>

```
┌──────────────────────────────────────────────────────┐
│ jayant@terminal:~$ whoami                             │
│ AI Engineer. Ex-Flutter developer.                    │
│ Builds LLM systems that work in production,           │
│ not just in a notebook.                                │
└──────────────────────────────────────────────────────┘
```

<br/>

## `$ cat about.txt`

I started as a **Flutter developer** — where every crash and every millisecond of jank was my problem in production, not in a notebook.

That discipline followed me into AI.

Most engineers enter AI through research and learn production discipline the hard way, after something breaks live. I came the other direction — I already knew what "in production" costs, and I bring that standard to every model, pipeline, and agent I build.

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
Retrieval-grounded Q&amp;A over a custom knowledge base, built to minimize hallucination rather than just demo well on easy queries.
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
| Backend &amp; APIs | Python · REST APIs |
| Data &amp; Query | SQL · Pandas · NumPy |
| Mobile (background) | Flutter · Dart |
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

## `$ history | tail -5`

```
001  flutter build --release        # shipped production mobile apps
002  pip install langchain          # started the shift to AI
003  python build_rag_pipeline.py   # built retrieval + citations
004  python run_agent.py --goal     # built multi-step autonomous agent
005  status: hardening evaluation, targeting AI Engineer roles
```

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

![stats](https://github-readme-stats.vercel.app/api?username=YOUR_GITHUB_USERNAME&amp;show_icons=true&amp;theme=dark&amp;hide_border=true&amp;bg_color=000000&amp;title_color=39FF14&amp;icon_color=39FF14&amp;text_color=39FF14)
![streak](https://github-readme-streak-stats.herokuapp.com/?user=YOUR_GITHUB_USERNAME&amp;theme=dark&amp;hide_border=true&amp;background=000000&amp;ring=39FF14&amp;fire=39FF14&amp;currStreakLabel=39FF14)

</div>

<br/>

<div align="center">

```
┌──────────────────────────────────────────────────────┐
│ jayant@terminal:~$ echo "let's talk"                  │
│ Open to AI Engineer roles — end-to-end ownership,      │
│ not just prompt-tuning.                                │
└──────────────────────────────────────────────────────┘
```

[![LinkedIn](https://img.shields.io/badge/CONNECT_ON_LINKEDIN-000000?style=for-the-badge&amp;logo=linkedin&amp;logoColor=39FF14&amp;labelColor=000000)](https://www.linkedin.com/in/jayantbhatiaa)
[![Email](https://img.shields.io/badge/EMAIL_ME-000000?style=for-the-badge&amp;logo=gmail&amp;logoColor=39FF14&amp;labelColor=000000)](mailto:jayantbhatia44@gmail.com)

<br/>

![footer](https://capsule-render.vercel.app/api?type=blur&amp;color=0:0d1f0d,100:000000&amp;height=80&amp;section=footer)

</div>
