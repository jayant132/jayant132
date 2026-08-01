<div align="center">

<img src="https://capsule-render.vercel.app/api?type=blur&color=0:0B0F19,100:1E1B4B&height=250&section=header&text=JAYANT%20BHATIA&fontSize=46&fontColor=E5E7EB&desc=AI%20Engineer%20%E2%80%94%20systems%20that%20reason,%20retrieve%20%26%20act&descSize=16&descAlignY=62&fontAlignY=38&animation=fadeIn" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&pause=1800&color=A5B4FC&center=true&vCenter=true&width=620&lines=Building+LLM+systems+that+survive+production;RAG+pipelines+%C2%B7+AI+agents+%C2%B7+LangChain;From+mobile+engineering+to+AI+engineering" />

<br/>

<a href="https://www.linkedin.com/in/jayantbhatiaa"><img src="https://img.shields.io/badge/LinkedIn-000000?style=flat-square&logo=linkedin&logoColor=A5B4FC&labelColor=0B0F19" /></a>
<a href="mailto:jayantbhatia44@gmail.com"><img src="https://img.shields.io/badge/Email-000000?style=flat-square&logo=gmail&logoColor=A5B4FC&labelColor=0B0F19" /></a>
<a href="https://github.com/YOUR_GITHUB_USERNAME"><img src="https://img.shields.io/badge/GitHub-000000?style=flat-square&logo=github&logoColor=A5B4FC&labelColor=0B0F19" /></a>

<br/><br/>

`AI Engineering` &nbsp;·&nbsp; `LLM Systems` &nbsp;·&nbsp; `RAG` &nbsp;·&nbsp; `Autonomous Agents` &nbsp;·&nbsp; `Production ML`

</div>

<br/>

## The Shift

I started as a **Flutter developer** — where every crash, every millisecond of jank, was my problem in production, not in a notebook.

That discipline followed me into AI.

Most engineers enter AI through research and learn production discipline the hard way, after something breaks live. I came the other direction — I already knew what "in production" costs, and I bring that standard to every model, pipeline, and agent I build.

<br/>

## How a Request Moves Through My Systems

Rather than describe the RAG pipeline in prose, here's the actual shape of it:

```mermaid
flowchart LR
    A[User Query] --> B[Query Understanding]
    B --> C[Hybrid Retrieval]
    C --> D[Vector Store]
    C --> E[Re-ranking]
    D --> E
    E --> F[Context Assembly]
    F --> G[LLM Generation]
    G --> H{Grounded in Source?}
    H -->|Yes| I[Answer + Citations]
    H -->|No| J[Fallback / Clarify]
```

And the agent reasoning loop behind the automation system:

```mermaid
flowchart TD
    A[Goal Received] --> B[Plan Next Step]
    B --> C[Select Tool]
    C --> D[Execute Action]
    D --> E{Goal Complete?}
    E -->|No| F[Update Working Memory]
    F --> B
    E -->|Yes| G[Return Result]
```

*Design choices, not defaults: re-ranking exists because naive top-k retrieval was returning plausible-but-wrong context. The fallback branch exists because I'd rather the system say "I don't know" than hallucinate an answer.*

<br/>

## What I Build

<table width="100%">
<tr>
<td width="50%" valign="top">

**🔎 RAG-Based Intelligent Chatbot**

Retrieval-grounded Q&A over a custom knowledge base, built to minimize hallucination rather than just demo well on easy queries.

**Problem it solves:** generic LLMs don't know your org's data — and naive RAG returns confident nonsense. This pipeline prioritizes retrieval precision and traceable answers.

`LangChain` `LLMs` `Vector Retrieval` `Prompt Engineering`

</td>
<td width="50%" valign="top">

**⚙️ AI Agent Automation System**

An autonomous agent that plans across multiple steps, selects tools, and executes workflows with minimal human input.

**Problem it solves:** most "AI automation" is one prompt in a trench coat. This reasons about *what to do next*, not just what to say next.

`AI Agents` `Tool Use` `LLM Orchestration` `APIs`

</td>
</tr>
</table>

<br/>

## Stack

<table width="100%">
<tr><th align="left" width="22%">Domain</th><th align="left">Tools</th></tr>
<tr><td><b>AI Engineering</b></td><td>LLMs · LangChain · RAG · Prompt Engineering · AI Agents</td></tr>
<tr><td><b>Backend & APIs</b></td><td>Python · REST APIs</td></tr>
<tr><td><b>Data & Query</b></td><td>SQL · Pandas · NumPy</td></tr>
<tr><td><b>Mobile (background)</b></td><td>Flutter · Dart</td></tr>
<tr><td><b>Tooling</b></td><td>Git · GitHub</td></tr>
</table>

<br/>

## How I Work

| Principle | In practice |
|---|---|
| **Ship over demo** | A pipeline that works on 3 curated questions isn't done — it's a prototype. |
| **Traceable AI** | If a system can't explain *why* it answered something, I don't trust it in production. |
| **Engineering first** | Latency, cost, and failure modes matter as much as model choice. |
| **Narrow and reliable beats broad and flaky** | I'd rather ship an agent that reliably does one thing than one that sometimes does five. |

<br/>

## Roadmap

```mermaid
timeline
    title From Mobile to AI Engineering
    Flutter Development : Shipped production mobile apps : Learned to own real-world reliability
    Transition : Studied LLMs, RAG, agentic systems : Rebuilt engineering habits around AI
    RAG & Agents : Built retrieval pipeline : Built multi-step autonomous agent
    Now : Hardening evaluation & reliability : Targeting production AI Engineer roles
```

<br/>

<details>
<summary><b>Currently exploring</b> (click to expand)</summary>
<br/>

- Hybrid retrieval — combining dense + sparse search for better recall on ambiguous queries
- Agent evaluation — moving past "it worked in my test run" toward measurable reliability
- Multi-agent coordination — where a single agent's context window becomes the bottleneck
- Cost-aware LLM architecture — same output quality, lower latency and spend

</details>

<br/>

## GitHub Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=YOUR_GITHUB_USERNAME&show_icons=true&theme=dark&hide_border=true&bg_color=0B0F19&title_color=A5B4FC&icon_color=A5B4FC&text_color=E5E7EB" height="165"/>
<img src="https://github-readme-streak-stats.herokuapp.com/?user=YOUR_GITHUB_USERNAME&theme=dark&hide_border=true&background=0B0F19&ring=A5B4FC&fire=A5B4FC&currStreakLabel=A5B4FC" height="165"/>

</div>

<br/>

<div align="center">

## Let's Talk

Open to **AI Engineer** roles where I can own systems end-to-end — not just tune prompts.

<a href="https://www.linkedin.com/in/jayantbhatiaa"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-000000?style=for-the-badge&logo=linkedin&logoColor=A5B4FC&labelColor=0B0F19" /></a>
<a href="mailto:jayantbhatia44@gmail.com"><img src="https://img.shields.io/badge/Email_Me-000000?style=for-the-badge&logo=gmail&logoColor=A5B4FC&labelColor=0B0F19" /></a>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=blur&color=0:1E1B4B,100:0B0F19&height=90&section=footer" width="100%"/>

</div>
