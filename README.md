<!--
  Profile README for github.com/Sachin-Gupta85
  Renders at the top of your GitHub profile. Edit the CONTACT section
  placeholders (LinkedIn / email) before you push — I left them blank on purpose.
-->

<div align="center">

<a href="https://github.com/Sachin-Gupta85">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1000&color=6F42C1&center=true&vCenter=true&width=820&lines=Sachin+Gupta;AI+Agent+Evaluation+%26+Benchmark+Engineer;LLM+Platform+%2B+Infrastructure;Deterministic%2C+tested%2C+reproducible+by+default" alt="Sachin Gupta" />
</a>

<p>
  <b>AI Engineer — Agent Evaluation • Benchmark Design • LLM Infrastructure</b><br/>
  I build evaluation harnesses and LLM platform systems that are <b>runnable, deterministic, and actually tested</b> —
  not slideware. Every repo here ships a reference solution and a passing test suite.
</p>

<p>
  <img src="https://img.shields.io/badge/focus-Agent%20Evals%20%2B%20LLM%20Infra-6f42c1?style=for-the-badge" />
  <img src="https://img.shields.io/badge/style-deterministic%20%7C%20offline%20%7C%20tested-2ea44f?style=for-the-badge" />
  <img src="https://komarev.com/ghpvc/?username=Sachin-Gupta85&style=for-the-badge&color=6f42c1&label=Profile+Views" />
</p>

</div>

---

## 🧭 About

- 🔬 **Agent & LLM evaluation** — Terminal-Bench task suites, LLM-as-judge harnesses, statistically-rigorous eval platforms (bootstrap CIs, significance testing, position-bias control).
- 🛠️ **LLM platform engineering** — resilient gateways, observability, durable agent orchestration, RAG systems, MCP tool servers.
- 🧱 **Full-stack delivery** — React + FastAPI and MERN apps with real test harnesses (not empty scaffolds).
- 🎯 **Operating principle** — if a reviewer can't `git clone && pytest` it and watch it pass, it doesn't ship. **Oracle passes, baseline fails, every claim is verifiable.**

---

## 🧪 Flagship — Benchmark & Evaluation Suites

> Real, graded, reproducible. Each number below is the repo's actual passing test count.

| Benchmark area | Repo | What it does | Tests |
|---|---|---|---|
| **LLM eval (statistics)** | [`llm-eval-platform`](https://github.com/Sachin-Gupta85/llm-eval-platform) | Bootstrap CIs, paired-bootstrap significance, pairwise A/B with **position-bias control**, self-consistency judge, CI regression gate | ✅ 15 |
| **LLM eval (metrics)** | [`llm-eval-harness`](https://github.com/Sachin-Gupta85/llm-eval-harness) | Exact-match / token-F1 / embedding-cosine / LLM-as-judge + Markdown report | ✅ 7 |
| **RAG eval** | [`rag-eval-platform`](https://github.com/Sachin-Gupta85/rag-eval-platform) | IR ranking metrics (recall@k, MRR, nDCG) **+** grounding (faithfulness, context-recall) with CIs | ✅ 19 |
| **Terminal / CLI agents** | [`tbench-terminal-1-logtop`](https://github.com/Sachin-Gupta85/tbench-terminal-1-logtop) · [`-2-dedup`](https://github.com/Sachin-Gupta85/tbench-terminal-2-dedup) · [`-3-csvagg`](https://github.com/Sachin-Gupta85/tbench-terminal-3-csvagg) · [`-4-maze`](https://github.com/Sachin-Gupta85/tbench-terminal-4-maze) | 16 Terminal-Bench 3 tasks graded on held-out cases | ✅ oracle=1/nop=0 |
| **SWE-bench style** | [`tbench-swe-task`](https://github.com/Sachin-Gupta85/tbench-swe-task) | Planted-bug fix tasks with hidden graders | ✅ 4 tasks |
| **Long-horizon agents** | [`tbench-longhorizon-task`](https://github.com/Sachin-Gupta85/tbench-longhorizon-task) | Engine-building tasks (spreadsheet engine, mini-VM, regex matcher) | ✅ 4 tasks |
| **Algorithms / Systems / ML** | [`tbench-algorithms`](https://github.com/Sachin-Gupta85/tbench-algorithms) · [`tbench-systems`](https://github.com/Sachin-Gupta85/tbench-systems) · [`tbench-ml-training`](https://github.com/Sachin-Gupta85/tbench-ml-training) | Exact algorithm, OS-sim, and from-scratch ML training tasks | ✅ 12 tasks |
| **RLVR / verifiable rewards** | [`rlvr-verifiers`](https://github.com/Sachin-Gupta85/rlvr-verifiers) | Answer extraction + exact math verification (no SymPy) + reward shaping | ✅ 17 |
| **Reasoning audit** | [`cot-reasoning-auditor`](https://github.com/Sachin-Gupta85/cot-reasoning-auditor) | Chain-of-thought checks: arithmetic, contradiction, answer-consistency, grounding | ✅ 17 |
| **GAIA-style agents** | [`gaia-agent-eval`](https://github.com/Sachin-Gupta85/gaia-agent-eval) | Faithful GAIA scorer, offline tools, per-level accuracy + tool coverage | ✅ 10 |
| **Safety / red-team** | [`model-redteam-harness`](https://github.com/Sachin-Gupta85/model-redteam-harness) | Refusal classifier + per-category Attack Success Rate (defensive) | ✅ 10 |
| **Observability** | [`llm-observability`](https://github.com/Sachin-Gupta85/llm-observability) | Span tracing, cost accounting, p95/p99, error taxonomy, regression gate | ✅ 26 |

> 📚 **Field map:** [`awesome-ai-evaluations`](https://github.com/Sachin-Gupta85/awesome-ai-evaluations) — a curated guide to LLM/agent benchmarks, methodology, statistics, safety, and frameworks.

---

## 🏗️ LLM Platform & Agent Infrastructure

| Repo | What it is | Tests |
|---|---|---|
| [`llm-gateway`](https://github.com/Sachin-Gupta85/llm-gateway) | Resilient gateway: policy routing + fallback, rate limiting, circuit breaker, jittered retry, semantic cache, budgets | ✅ 31 |
| [`agent-orchestrator`](https://github.com/Sachin-Gupta85/agent-orchestrator) | Durable DAG engine: checkpoint/resume, **exactly-once replay**, saga compensation | ✅ 16 |
| [`langgraph-sql-assistant`](https://github.com/Sachin-Gupta85/langgraph-sql-assistant) | NL→SQL with a read-only safety gate and a validate/repair loop | ✅ 8 |
| [`langchain-rag-advanced`](https://github.com/Sachin-Gupta85/langchain-rag-advanced) | Hybrid BM25+dense retrieval, Reciprocal Rank Fusion, cited answers | ✅ 8 |
| [`langgraph-research-agent`](https://github.com/Sachin-Gupta85/langgraph-research-agent) | Plan → research → draft → critique → revise state machine | ✅ 4 |
| [`react-tool-agent`](https://github.com/Sachin-Gupta85/react-tool-agent) | ReAct tool-calling loop: tool registry, JSON decisions, step guards | ✅ 8 |
| [`mcp-toolbox-server`](https://github.com/Sachin-Gupta85/mcp-toolbox-server) | MCP (FastMCP) server exposing safe calculator / text / units / SQL tools | ✅ 9 |
| [`agentic-rag`](https://github.com/Sachin-Gupta85/agentic-rag) | Self-correcting RAG agent (routing, doc grading, query rewrite) on LangGraph | — |

---

## 💻 Full-Stack Apps (real, with test harnesses)

**React + FastAPI + MongoDB:** [`notes`](https://github.com/Sachin-Gupta85/fastapi-react-notes) · [`bookmarks`](https://github.com/Sachin-Gupta85/fastapi-react-bookmarks) · [`polls`](https://github.com/Sachin-Gupta85/fastapi-react-polls) · [`recipes`](https://github.com/Sachin-Gupta85/fastapi-react-recipes) · [`habit-tracker`](https://github.com/Sachin-Gupta85/fastapi-react-habit-tracker)
**MERN + Python tool:** [`task-board`](https://github.com/Sachin-Gupta85/mern-task-board) · [`expense-tracker`](https://github.com/Sachin-Gupta85/mern-expense-tracker) · [`url-shortener`](https://github.com/Sachin-Gupta85/mern-url-shortener) · [`blog-platform`](https://github.com/Sachin-Gupta85/mern-blog-platform) · [`snippet-vault`](https://github.com/Sachin-Gupta85/mern-snippet-vault)
**RAG apps:** [`rag-pdf-chatbot`](https://github.com/Sachin-Gupta85/rag-pdf-chatbot) · [`rag-website-qa`](https://github.com/Sachin-Gupta85/rag-website-qa)

<sub>Every full-stack repo ships pytest + Jest/Vitest and docker-compose — tested, not empty.</sub>

---

## 🧰 Tech Stack

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/LangGraph-6f42c1?style=flat-square" />
  <img src="https://img.shields.io/badge/MCP-000000?style=flat-square" />
  <img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white" />
</p>
<p>
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white" />
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" />
  <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
</p>

---

## 📊 GitHub Stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=Sachin-Gupta85&show_icons=true&hide_border=true&title_color=6f42c1&icon_color=6f42c1&count_private=true" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Sachin-Gupta85&layout=compact&hide_border=true&title_color=6f42c1&langs_count=8" />

<br/>

<img src="https://streak-stats.demolab.com?user=Sachin-Gupta85&hide_border=true&ring=6f42c1&fire=6f42c1&currStreakLabel=6f42c1" />

<br/>

<img src="https://github-profile-trophy.vercel.app/?username=Sachin-Gupta85&theme=nord&no-frame=true&column=7&margin-w=5" />

</div>

---

## 📫 Contact

<p>
  <a href="https://www.linkedin.com/in/saching85/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:saching852002@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  <a href="https://github.com/Sachin-Gupta85">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
</p>

- 🔗 LinkedIn: [in/saching85](https://www.linkedin.com/in/saching85/)
- ✉️ Email: [saching852002@gmail.com](mailto:saching852002@gmail.com)
- 💻 GitHub: [@Sachin-Gupta85](https://github.com/Sachin-Gupta85)

<div align="center">
<sub>Every repo in this profile is runnable and tested. Clone any of them and watch the suite pass. 🟢</sub>
</div>
