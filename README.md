<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1,6,11,20&height=220&section=header&text=Sachin%20Gupta&fontSize=52&fontColor=ffffff&animation=fadeIn&subtext=AI%20Engineer%20%E2%80%A2%20Agent%20Benchmarks%20%E2%80%A2%20LLM%20Infrastructure%20%E2%80%A2%20RLVR&subfontSize=18&subfontColor=d8b4fe" width="100%" />

  [![Gmail](https://img.shields.io/badge/Gmail-saching852002%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:saching852002@gmail.com)
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-in%2Fsaching85-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/saching85/)
  [![GitHub](https://img.shields.io/badge/GitHub-Sachin--Gupta85-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Sachin-Gupta85)
  [![Status](https://img.shields.io/badge/Open_to-AI_Eval_%26_LLM_Infra_Work-00C853?style=for-the-badge)]()

  <br /><br />

  ```text
  $ whoami
  > Sachin Gupta — AI Engineer · Agent Evaluation & Benchmark Design
  > Building deterministic, tested eval harnesses for SWE-bench / TerminalBench / GAIA / RLVR-style tasks
  ```
</div>

---

### ⚡ At a Glance

<div align="center">
  <img src="https://img.shields.io/badge/Evaluation_%26_Infra_Repos-16+-4F46E5?style=flat-square&logo=github" />
  <img src="https://img.shields.io/badge/Passing_Tests-200+_across_repos-10B981?style=flat-square&logo=pytest" />
  <img src="https://img.shields.io/badge/Harnesses-Deterministic_%7C_Offline-0284C7?style=flat-square&logo=python" />
  <img src="https://img.shields.io/badge/Grading-Oracle%3D1_%2F_Nop%3D0-F59E0B?style=flat-square&logo=speedtest" />
  <img src="https://img.shields.io/badge/Sandboxing-Docker_Isolated-7928CA?style=flat-square&logo=docker" />
</div>

---

## 🔬 Core Focus & Engineering Specialization

I specialize in **AI agent evaluation, deterministic grading harnesses, and benchmark task design**. My work centers on building rigorous, verifiable tasks and evaluation infrastructure that stress multi-step agentic trajectories and code intelligence. **Every harness runs offline with deterministic reference solutions** — so a reviewer can `git clone && pytest` and watch the suite pass without an API key.

- 🎯 **Long-Horizon Agent Tasks (15–30+ steps):** Multi-turn engine-building environments (spreadsheet engine, bytecode VM, regex matcher) that test context retention, backtracking, and multi-file code synthesis.
- 💻 **Terminal & OS Benchmarks (Terminal-Bench style):** Linux/CLI debugging and data-processing tasks graded in isolated Docker containers with deterministic pytest assertions (Oracle solution passes, stub fails).
- 🛠️ **SWE-bench-Style Task Creation:** Planted-bug fix tasks with hidden Fail-to-Pass / Pass-to-Pass graders and strict test/patch separation.
- 🧪 **RLVR (Verifiable Rewards):** Deterministic reward environments where model outputs are checked programmatically — no human ambiguity, no heavyweight SymPy.
- 🚨 **Model Red-Teaming (Defensive):** Structural attack-category probes with placeholder payloads and per-category Attack Success Rate scoring for refusal-robustness evaluation.

---

## 🏗️ Evaluation Harness Architecture

```
                 ┌──────────────────────────────────────┐
                 │  Problem Definition & Target State   │
                 └──────────────────┬───────────────────┘
                                    │
                                    ▼
       ┌────────────────────────────────────────────────────────┐
       │             Isolated Sandbox Execution                 │
       │  • Ephemeral Docker Container (Ubuntu/Alpine)          │
       │  • Corrupt State Injection (Git/Sysadmin/Networking)   │
       │  • Strict Non-Interactive Environment Boundaries       │
       └────────────────────────────┬───────────────────────────┘
                                    │
                         Observation Loop (Tool Execution)
                                    │
                                    ▼
       ┌────────────────────────────────────────────────────────┐
       │             Autonomous Agent Reasoning                 │
       │  • Multi-Turn Tool Loop (ReAct / Function Calling)     │
       │  • Trajectory Telemetry (Tokens, Latency, Commands)    │
       └────────────────────────────┬───────────────────────────┘
                                    │
                        Completion Signal (EXIT)
                                    │
                                    ▼
       ┌────────────────────────────────────────────────────────┐
       │            Deterministic Grading Engine                │
       │  • Fail-to-Pass (F2P) & Pass-to-Pass (P2P) Assertions  │
       │  • Negative Constraint Violation Auditor               │
       │  • Exit Code & File System Integrity Check             │
       └────────────────────────────┬───────────────────────────┘
                                    │
                                    ▼
                  [Pass@1 Report & Cognitive Metrics]
```

---

## 🏆 Flagship Evaluation Suites & Benchmarks

<table>
  <tr>
    <td width="50%">
      <h3 align="center">🖥️ <a href="https://github.com/Sachin-Gupta85/tbench-terminal-1-logtop">Terminal-Bench Task Suites</a></h3>
      <p align="center"><b>Sandboxed CLI & OS Agent Benchmark Harness (16 Tasks)</b></p>
      <ul>
        <li><b>16 Tasks:</b> Text/log parsing (<a href="https://github.com/Sachin-Gupta85/tbench-terminal-1-logtop">1-logtop</a>), filesystem deduplication (<a href="https://github.com/Sachin-Gupta85/tbench-terminal-2-dedup">2-dedup</a>), CSV aggregation (<a href="https://github.com/Sachin-Gupta85/tbench-terminal-3-csvagg">3-csvagg</a>), BFS maze navigation (<a href="https://github.com/Sachin-Gupta85/tbench-terminal-4-maze">4-maze</a>).</li>
        <li><b>Sandboxing:</b> Isolated Docker & subprocess execution; every task verified Oracle=1 / Nop=0.</li>
        <li><b>Format:</b> Terminal-Bench 3 standard with hidden grading scripts.</li>
      </ul>
      <p align="center">
        <img src="https://img.shields.io/badge/Tasks-16_Verified-brightgreen" />
        <img src="https://img.shields.io/badge/Grading-Oracle%3D1_%2F_Nop%3D0-blue" />
      </p>
    </td>
    <td width="50%">
      <h3 align="center">🛠️ <a href="https://github.com/Sachin-Gupta85/tbench-swe-task">tbench-swe-task</a></h3>
      <p align="center"><b>SWE-bench-Style Bug-Fix Tasks for Coding Agents</b></p>
      <ul>
        <li><b>4 Tasks:</b> Planted bugs across Python packages with hidden test graders.</li>
        <li><b>Patch Purity:</b> Enforces strict separation between test patches and code fixes.</li>
        <li><b>Grading:</b> Fail-to-Pass (F2P) and Pass-to-Pass (P2P) assertions on held-out runs.</li>
      </ul>
      <p align="center">
        <img src="https://img.shields.io/badge/Format-SWE--bench_Style-orange" />
        <img src="https://img.shields.io/badge/F2P%2FP2P-Enforced-success" />
      </p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3 align="center">🧠 <a href="https://github.com/Sachin-Gupta85/tbench-longhorizon-task">tbench-longhorizon-task</a></h3>
      <p align="center"><b>Long-Horizon Agent Engine-Building Tasks</b></p>
      <ul>
        <li><b>15–30+ Step Tasks:</b> Spreadsheet formula engine, mini bytecode VM, regex matcher.</li>
        <li><b>Stress Testing:</b> Architectural coherence, edge-case recovery, multi-file code synthesis.</li>
        <li><b>Scoring:</b> Hidden test suites; every task Oracle=1 / Nop=0.</li>
      </ul>
      <p align="center">
        <img src="https://img.shields.io/badge/Horizon-15--30%2B_Steps-red" />
        <img src="https://img.shields.io/badge/Tasks-4_Engines-purple" />
      </p>
    </td>
    <td width="50%">
      <h3 align="center">🧮 <a href="https://github.com/Sachin-Gupta85/rlvr-verifiers">rlvr-verifiers</a></h3>
      <p align="center"><b>RLVR Deterministic Reward Environments</b></p>
      <ul>
        <li><b>Verifiable Rewards:</b> Deterministic reward functions (r ∈ {0.0, 1.0}) for reasoning models.</li>
        <li><b>Pure Python:</b> Exact math extraction without SymPy; robust fraction/boxed-answer parsing.</li>
        <li><b>Reward Shaping:</b> Format-compliance bonus and partial credit; 17 unit tests.</li>
      </ul>
      <p align="center">
        <img src="https://img.shields.io/badge/RLVR-Binary_Rewards-brightgreen" />
        <img src="https://img.shields.io/badge/Tests-17_Passing-blue" />
      </p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3 align="center">🌍 <a href="https://github.com/Sachin-Gupta85/gaia-agent-eval">gaia-agent-eval</a></h3>
      <p align="center"><b>GAIA-Style Agent Evaluation Harness</b></p>
      <ul>
        <li><b>Levels 1–3 Scorer:</b> Faithful GAIA quasi-exact scoring (number normalise, order-independent list match).</li>
        <li><b>Offline Tool Registry:</b> Deterministic calculator, search, and file-reader fixtures.</li>
        <li><b>Metrics:</b> Per-level accuracy and tool-usage coverage; 10 passing tests.</li>
      </ul>
      <p align="center">
        <img src="https://img.shields.io/badge/Benchmark-GAIA-purple" />
        <img src="https://img.shields.io/badge/Tests-10_Passing-blue" />
      </p>
    </td>
    <td width="50%">
      <h3 align="center">🔬 <a href="https://github.com/Sachin-Gupta85/cot-reasoning-auditor">cot-reasoning-auditor</a></h3>
      <p align="center"><b>Chain-of-Thought Logical Coherence Auditor</b></p>
      <ul>
        <li><b>Trace Auditing:</b> Arithmetic consistency, logical contradiction, and answer-grounding checks.</li>
        <li><b>Grounding Rule:</b> Flags answers that are declared but never derived in the work.</li>
        <li><b>Verification:</b> Validated on constructed CoT traces with injected errors; 17 passing tests.</li>
      </ul>
      <p align="center">
        <img src="https://img.shields.io/badge/Focus-CoT%20Auditing-orange" />
        <img src="https://img.shields.io/badge/Tests-17_Passing-brightgreen" />
      </p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3 align="center">🛡️ <a href="https://github.com/Sachin-Gupta85/model-redteam-harness">model-redteam-harness</a></h3>
      <p align="center"><b>Adversarial Red-Teaming & Safety Suite (Defensive)</b></p>
      <ul>
        <li><b>Structural Probes:</b> 6 attack categories built from templates with placeholder payloads (no real exploits).</li>
        <li><b>Refusal Classifier:</b> Lexical refusal/compliance detector for defensibility scoring.</li>
        <li><b>ASR Telemetry:</b> Per-category Attack Success Rate scoring; 10 passing tests.</li>
      </ul>
      <p align="center">
        <img src="https://img.shields.io/badge/Vectors-Structural_Probes-red" />
        <img src="https://img.shields.io/badge/Tests-10_Passing-teal" />
      </p>
    </td>
    <td width="50%">
      <h3 align="center">📊 <a href="https://github.com/Sachin-Gupta85/llm-eval-platform">llm-eval-platform</a></h3>
      <p align="center"><b>Statistically-Rigorous LLM Evaluation Platform</b></p>
      <ul>
        <li><b>Bootstrap Statistics:</b> 95% bootstrap confidence intervals and paired-bootstrap significance testing.</li>
        <li><b>Bias Control:</b> Pairwise A/B judging with position-bias counterbalancing and self-consistency vote.</li>
        <li><b>CI Gate:</b> Non-regression gate that fails a build only on a statistically significant drop; 15 tests.</li>
      </ul>
      <p align="center">
        <img src="https://img.shields.io/badge/Statistics-Bootstrap_CIs-blue" />
        <img src="https://img.shields.io/badge/Tests-15_Passing-brightgreen" />
      </p>
    </td>
  </tr>
</table>

---

## 🏗️ LLM Platform & Infrastructure Showcase

| Repository | Focus & Architecture | Tests |
| :--- | :--- | :---: |
| [`llm-gateway`](https://github.com/Sachin-Gupta85/llm-gateway) | Resilient LLM gateway: policy routing + fallback, token-bucket rate limiting, circuit breaker, semantic caching, budgets | ✅ 31 pytest |
| [`agent-orchestrator`](https://github.com/Sachin-Gupta85/agent-orchestrator) | Durable DAG engine: checkpoint/resume, deterministic replay (exactly-once), saga compensation rollback | ✅ 16 pytest |
| [`rag-eval-platform`](https://github.com/Sachin-Gupta85/rag-eval-platform) | RAG evaluation: IR ranking metrics (Recall@k, MRR, nDCG) + grounding (faithfulness, context recall) with CIs | ✅ 19 pytest |
| [`llm-observability`](https://github.com/Sachin-Gupta85/llm-observability) | LLM observability: span tracing, token-to-cost accounting, p95/p99 latency percentiles, regression gate | ✅ 26 pytest |
| [`mcp-toolbox-server`](https://github.com/Sachin-Gupta85/mcp-toolbox-server) | MCP (FastMCP) server exposing safe calculator, text transform, units conversion, and read-only SQL tools | ✅ 9 pytest |
| [`langgraph-sql-assistant`](https://github.com/Sachin-Gupta85/langgraph-sql-assistant) | LangGraph NL→SQL over SQLite with a read-only safety gate and self-repair loop | ✅ 8 pytest |
| [`langchain-rag-advanced`](https://github.com/Sachin-Gupta85/langchain-rag-advanced) | Advanced RAG: hybrid BM25 + dense retrieval, Reciprocal Rank Fusion, source-cited FastAPI service | ✅ 8 pytest |
| [`react-tool-agent`](https://github.com/Sachin-Gupta85/react-tool-agent) | ReAct tool-calling loop: tool registry, JSON decisions, step guards, tool-error recovery | ✅ 8 pytest |
| [`langgraph-research-agent`](https://github.com/Sachin-Gupta85/langgraph-research-agent) | Plan → research → draft → critique → revise state machine on LangGraph | ✅ 4 pytest |
| [`llm-eval-harness`](https://github.com/Sachin-Gupta85/llm-eval-harness) | Provider-agnostic eval: exact-match / token-F1 / embedding-cosine / LLM-as-judge + Markdown report | ✅ 7 pytest |
| [`awesome-ai-evaluations`](https://github.com/Sachin-Gupta85/awesome-ai-evaluations) | Curated map of LLM/agent benchmarks, evaluation methodology, statistics, and safety frameworks | 📚 Resource |

> Also on the profile: full-stack apps (React + FastAPI + MongoDB, and MERN), each shipping pytest + Vitest/Jest and docker-compose.

---

## 🛠️ Technical Stack & Tooling

<div align="center">

| Layer | Technologies & Tooling |
| :--- | :--- |
| **Core Languages** | `Python 3.10+`, `TypeScript`, `JavaScript`, `Bash / Shell`, `SQL` |
| **Sandbox & Infrastructure** | `Docker`, `Linux Internals`, `Git`, `GitHub Actions`, `docker-compose` |
| **Testing & Determinism** | `Pytest`, `Subprocess Sandboxing`, `AST Analysis`, `Seeded RNG / Injected Clocks`, `Vitest / Jest` |
| **Agent Frameworks & SDKs** | `LangGraph`, `LangChain`, `FastMCP (Model Context Protocol)`, `Provider-Abstraction Pattern` |
| **Evaluation Methods** | `Terminal-Bench 3`, `SWE-bench-style F2P/P2P`, `GAIA scoring`, `RLVR`, `Bootstrap CIs / Position-Bias Control` |
| **Web & Applications** | `React 18`, `FastAPI`, `Next.js`, `TailwindCSS`, `MongoDB`, `Express` |

</div>

---

## 📈 GitHub Stats

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Sachin-Gupta85&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="Sachin's GitHub Stats" width="48%" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Sachin-Gupta85&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top Languages" width="48%" />
</div>

<div align="center">
<sub>Every repo above is runnable and tested — clone any of them and watch the suite pass. The stats cards render live from GitHub and reflect my real activity.</sub>
</div>

---

## 📬 Contact & Availability

- 💼 **Open to AI Evaluation, Benchmark Authoring, and LLM Platform engineering work.**
- ✉️ **Email:** **[saching852002@gmail.com](mailto:saching852002@gmail.com)**
- 🔗 **LinkedIn:** **[linkedin.com/in/saching85](https://www.linkedin.com/in/saching85/)**
- 🌐 **GitHub:** **[github.com/Sachin-Gupta85](https://github.com/Sachin-Gupta85)**

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1,6,11,20&height=100&section=footer" width="100%" />
</div>
