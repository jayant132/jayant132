<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1f0d,50:143d14,100:39FF14&height=220&section=header&text=JAYANT%20BHATIA&fontSize=48&fontColor=000000&fontAlignY=42&desc=AI%20Engineer%20%E2%80%94%20building%20systems%20that%20reason,%20retrieve%20%26%20act&descSize=16&descAlignY=62&animation=fadeIn" width="100%"/>

<a href="https://www.linkedin.com/in/jayantbhatiaa"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="mailto:jayantbhatia44@gmail.com"><img src="https://img.shields.io/badge/Email-000000?style=for-the-badge&logo=gmail&logoColor=39FF14" /></a>
<a href="https://github.com/jayant132"><img src="https://img.shields.io/badge/GitHub-000000?style=for-the-badge&logo=github&logoColor=39FF14" /></a>
<img src="https://img.shields.io/badge/Open_to_Work-39FF14?style=for-the-badge&logo=target&logoColor=000000" />

</div>

<br/>

> **For the recruiter with 15 seconds:** I build production-grade RAG pipelines and autonomous LLM agents — not notebook demos. Background in shipping real Flutter apps to real users means I think about latency, failure modes, and cost before I think about which model to use. Currently open to AI Engineer roles.

<br/>

<div align="center">

### `$ whoami --verbose`

</div>

I work at the layer where language models stop being a chat toy and start being **infrastructure** — systems that retrieve real information, cite it, and know when to say "I don't know" instead of hallucinating with confidence.

Before AI, I was a Flutter developer. That background isn't a footnote — it's why I default to asking "what happens when this breaks in production" before I ask "which model performs best on the benchmark."

<br/>

<div align="center">

### `$ cat architecture/`

</div>

**RAG Pipeline — designed to be *wrong less often*, not just fast**

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

**Agent Reasoning Loop — plans before it acts**

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

<sub>Design choices, not defaults — re-ranking exists because naive top-k retrieval returned plausible-but-wrong context. The fallback branch exists on purpose.</sub>

<br/>

<div align="center">

### `$ ls -la projects/`

</div>

<table>
<tr>
<td width="50%" valign="top">

**🔍 rag-chatbot**
Retrieval-grounded Q&A over a custom knowledge base — built to minimize hallucination, not just demo well on easy queries.

*Problem it solves:* generic LLMs don't know your org's data, and naive RAG returns confident nonsense.

`LangChain` `RAG` `Vector Retrieval` `Prompt Engineering`

[`→ view repo`](https://github.com/jayant132)

</td>
<td width="50%" valign="top">

**🤖 agent-automation**
An autonomous agent that plans across multiple steps, selects tools, and executes workflows with minimal human input.

*Problem it solves:* most "AI automation" is one prompt in a trench coat. This reasons about what to do next.

`AI Agents` `Tool Use` `LLM Orchestration` `APIs`

[`→ view repo`](https://github.com/jayant132)

</td>
</tr>
</table>

<sub>💡 Replace these repo links with your actual GitHub URLs once pushed.</sub>

<br/>

<div align="center">

### `$ cat stack.json`

<img src="https://skillicons.dev/icons?i=python,langchain,flutter,dart,git,github,vscode,postgres&theme=dark" />

<br/><br/>

| Domain | Tools |
|:--|:--|
| **AI Engineering** | LLMs · LangChain · RAG · Prompt Engineering · AI Agents |
| **Backend & APIs** | Python · REST APIs |
| **Data & Query** | SQL · Pandas · NumPy |
| **Also fluent in** | Flutter · Dart |

</div>

<br/>

<div align="center">

### `$ cat principles.md`

</div>

| Principle | In practice |
|:--|:--|
| **Ship over demo** | A pipeline that works on 3 curated questions isn't done — it's a prototype. |
| **Traceable AI** | If a system can't explain why it answered something, I don't trust it in production. |
| **Engineering first** | Latency, cost, and failure modes matter as much as model choice. |
| **Narrow & reliable > broad & flaky** | I'd rather ship one thing that always works than five that sometimes do. |

<br/>

<details>
<summary><b>$ cat currently_exploring.txt</b></summary>
<br/>

- **Hybrid retrieval** — combining dense + sparse search for better recall on ambiguous queries
- **Agent evaluation** — moving past "it worked in my test run" toward measurable reliability
- **Multi-agent coordination** — where a single agent's context window becomes the bottleneck
- **Cost-aware LLM architecture** — same output quality, lower latency and spend

</details>

<br/>

<div align="center">

### `$ fetch --stats`

<img src="https://github-readme-stats.vercel.app/api?username=jayant132&show_icons=true&theme=dark&hide_border=true&bg_color=00000000&title_color=39FF14&icon_color=39FF14&text_color=c9c9c9" height="165"/>
<img src="https://github-readme-streak-stats.herokuapp.com/?user=jayant132&theme=dark&hide_border=true&background=00000000&ring=39FF14&fire=39FF14&currStreakLabel=39FF14" height="165"/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=jayant132&layout=compact&theme=dark&hide_border=true&bg_color=00000000&title_color=39FF14&text_color=c9c9c9" />

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

<a href="https://www.linkedin.com/in/jayantbhatiaa"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="mailto:jayantbhatia44@gmail.com"><img src="https://img.shields.io/badge/Email_Me-000000?style=for-the-badge&logo=gmail&logoColor=39FF14" /></a>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:39FF14,50:143d14,100:0d1f0d&height=120&section=footer" width="100%"/>

</div>
