<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1,6,11,20&height=220&section=header&text=Sachin%20Gupta&fontSize=52&fontColor=ffffff&animation=fadeIn&subtext=AI%20Engineer%20%E2%80%A2%20Agent%20Benchmarks%20%E2%80%A2%20LLM%20Infrastructure%20%E2%80%A2%20RLVR&subfontSize=18&subfontColor=d8b4fe" width="100%" />

  [![Gmail](https://img.shields.io/badge/Gmail-saching852002%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:saching852002@gmail.com)
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-in%2Fsaching85-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/saching85/)
  [![GitHub](https://img.shields.io/badge/GitHub-Sachin--Gupta85-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Sachin-Gupta85)
  [![Status](https://img.shields.io/badge/Status-Open_for_AI_Eval_Contracts-00C853?style=for-the-badge)]()
  [![Mercor & Turing Ready](https://img.shields.io/badge/Platforms-Mercor_%7C_Turing_%7C_Scale_AI-7928CA?style=for-the-badge)]()

  <br />

  <!-- 🏆 Verified Achievements Quick-Bar -->
  <a href="https://github.com/Sachin-Gupta85?tab=achievements"><img src="https://img.shields.io/badge/Pull%20Shark-Silver-10B981?style=for-the-badge&logo=github&logoColor=white" alt="Pull Shark Silver" /></a>
  <a href="https://github.com/Sachin-Gupta85?tab=achievements"><img src="https://img.shields.io/badge/Quickdraw-Unlocked-F59E0B?style=for-the-badge&logo=lightning&logoColor=white" alt="Quickdraw" /></a>
  <a href="https://github.com/Sachin-Gupta85?tab=achievements"><img src="https://img.shields.io/badge/YOLO-Merged-EF4444?style=for-the-badge&logo=gitpullrequest&logoColor=white" alt="YOLO" /></a>
  <a href="https://github.com/Sachin-Gupta85?tab=achievements"><img src="https://img.shields.io/badge/Galaxy%20Brain-Silver-8B5CF6?style=for-the-badge&logo=githubdiscussions&logoColor=white" alt="Galaxy Brain Silver" /></a>
  <a href="https://github.com/Sachin-Gupta85?tab=achievements"><img src="https://img.shields.io/badge/Pair%20Extraordinaire-Bronze-06B6D4?style=for-the-badge&logo=github&logoColor=white" alt="Pair Extraordinaire" /></a>

  <br /><br />

  ```text
  $ whoami
  > Sachin Gupta — Frontier AI Engineer & Agent Benchmark Specialist
  > Specializing in SWE-bench, TerminalBench, GAIA, RLVR Verifiers & Long-Horizon Failures
  ```
</div>

---

### ⚡ At a Glance

<div align="center">
  <img src="https://img.shields.io/badge/Benchmark_Suites-12_Production_Frameworks-4F46E5?style=flat-square&logo=github" />
  <img src="https://img.shields.io/badge/Verification_Standard-100%25_Deterministic-10B981?style=flat-square&logo=pytest" />
  <img src="https://img.shields.io/badge/Adversarial_Vectors-250%2B_Red--Team_Probes-EF4444?style=flat-square&logo=securityscorecard" />
  <img src="https://img.shields.io/badge/Long--Horizon_Tasks-15--30%2B_Steps-F59E0B?style=flat-square&logo=speedtest" />
  <img src="https://img.shields.io/badge/Infrastructure-Docker_Sandboxed-0284C7?style=flat-square&logo=docker" />
</div>

---

## 🔬 Core Focus & Engineering Specialization

I specialize in **frontier AI evaluation, deterministic grading harnesses, and agent task synthesis**. My work centers on creating rigorous, verifiable tasks that frontier models (GPT-4o, Claude 3.5 Sonnet, DeepSeek-R1/V3, Gemini 1.5/2.0) fail on—specifically in multi-step agentic trajectories and code intelligence.

- 🎯 **Long-Horizon Agent Trajectories (15–30+ steps):** Designing multi-turn interactive environments testing context retention, backtracking, tool error recovery, and constraint stability.
- 💻 **Terminal & OS Benchmarks (TerminalBench / OSWorld style):** Authoring realistic Linux/CLI debugging scenarios, system administration puzzles, and network edge cases evaluated with isolated Docker containers and deterministic pytest assertions.
- 🛠️ **SWE-bench Task Creation:** Extracting real-world GitHub issues and PRs into standardized SWE-bench instances (clean base commit, problem statement, reproducible fail-to-pass test patches).
- 🧪 **RLVR (Reinforcement Learning with Verifiable Rewards):** Engineering automated deterministic grading environments where model outputs can be verified programmatically without human ambiguity.
- 🚨 **Model Red-Teaming & Failure Taxonomy:** Systematic failure mode categorization (sycophancy, context window degradation, tool loop hallucination, subtle numerical/boundary drift).

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
        <li><b>16 Production Tasks:</b> Text/log parsing (<a href="https://github.com/Sachin-Gupta85/tbench-terminal-1-logtop">1-logtop</a>), filesystem deduplication (<a href="https://github.com/Sachin-Gupta85/tbench-terminal-2-dedup">2-dedup</a>), CSV aggregation (<a href="https://github.com/Sachin-Gupta85/tbench-terminal-3-csvagg">3-csvagg</a>), BFS maze grid navigation (<a href="https://github.com/Sachin-Gupta85/tbench-terminal-4-maze">4-maze</a>).</li>
        <li><b>Sandboxing:</b> Isolated Docker & subprocess execution with 100% reference Oracle verification.</li>
        <li><b>Format:</b> Terminal-Bench 3 standard with hidden grading scripts.</li>
      </ul>
      <p align="center">
        <img src="https://img.shields.io/badge/Tasks-16_Verified-brightgreen" />
        <img src="https://img.shields.io/badge/Pass%401-Oracle%3D1.0-blue" />
      </p>
    </td>
    <td width="50%">
      <h3 align="center">🛠️ <a href="https://github.com/Sachin-Gupta85/tbench-swe-task">tbench-swe-task</a></h3>
      <p align="center"><b>SWE-bench Bug-Fix Tasks for Coding Agents</b></p>
      <ul>
        <li><b>4 SWE-bench Tasks:</b> Planted bugs across production Python packages with hidden test graders.</li>
        <li><b>Patch Purity:</b> Rigorous check enforcing strict separation between test patches and code fixes.</li>
        <li><b>Grading:</b> Fail-to-Pass (F2P) and Pass-to-Pass (P2P) assertions on held-out test runs.</li>
      </ul>
      <p align="center">
        <img src="https://img.shields.io/badge/Format-Official_SWE--bench-orange" />
        <img src="https://img.shields.io/badge/F2P%2FP2P-Enforced-success" />
      </p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3 align="center">🧠 <a href="https://github.com/Sachin-Gupta85/tbench-longhorizon-task">tbench-longhorizon-task</a></h3>
      <p align="center"><b>Long-Horizon Agent Engine-Building Tasks</b></p>
      <ul>
        <li><b>15–30+ Step Tasks:</b> Spreadsheet formula engine, mini bytecode VM, JSONPath query engine, and regex matcher.</li>
        <li><b>Stress Testing:</b> Tests architectural coherence, edge-case recovery, and multi-file code synthesis.</li>
        <li><b>Scoring:</b> Hidden test suites with property-based randomized test inputs.</li>
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
        <li><b>Verifiable Rewards:</b> Deterministic reward functions ($r \in \{0.0, 1.0\}$) for reasoning models (PPO/GRPO).</li>
        <li><b>Pure Python Engine:</b> Exact math extraction without heavyweight SymPy dependencies; robust fraction/radical parsing.</li>
        <li><b>Reward Shaping:</b> Length penalties, format compliance checks, and partial credit modes; 17 unit tests.</li>
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
      <p align="center"><b>GAIA-Style Multi-Modal Agent Evaluation Harness</b></p>
      <ul>
        <li><b>Levels 1–3 Scorer:</b> Faithful implementation of GAIA quasi-exact evaluation matching official rules.</li>
        <li><b>Offline Tool Registry:</b> Web search, Python shell, and file reader mocks with deterministic fixtures.</li>
        <li><b>Metrics:</b> Per-level accuracy, tool usage coverage, trajectory cost telemetry; 10 passing tests.</li>
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
        <li><b>Reasoning Trace Auditing:</b> Arithmetic consistency, logical contradiction, and answer grounding checks.</li>
        <li><b>Backtrack Scoring:</b> Evaluates self-correction efficacy and overthinking token penalties.</li>
        <li><b>Verification:</b> Tested against reasoning traces from frontier models; 17 passing tests.</li>
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
      <p align="center"><b>Adversarial Red-Teaming & Safety Suite</b></p>
      <ul>
        <li><b>Structural Probes:</b> Indirect prompt injection, jailbreak classification, and sycophancy detectors.</li>
        <li><b>Refusal Classifier:</b> Fast regex + heuristic refusal detector for defensibility scoring.</li>
        <li><b>ASR Telemetry:</b> Per-category Attack Success Rate (ASR) scoring across 10 passing test suites.</li>
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
        <li><b>Bootstrap Statistics:</b> 95% bootstrap confidence intervals, paired-bootstrap significance testing.</li>
        <li><b>Bias Control:</b> Pairwise A/B testing with position-bias counterbalancing and self-consistency judge.</li>
        <li><b>CI Gate:</b> Automated non-regression gate failing builds when accuracy drops below threshold; 15 tests.</li>
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

| Repository | Focus & Architecture | Passing Tests |
| :--- | :--- | :---: |
| [`llm-gateway`](https://github.com/Sachin-Gupta85/llm-gateway) | Resilient LLM gateway: policy routing + fallback, token-bucket rate limiting, circuit breaker, semantic caching, budgets | ✅ 31 pytest |
| [`agent-orchestrator`](https://github.com/Sachin-Gupta85/agent-orchestrator) | Durable DAG engine: checkpoint/resume, deterministic replay (exactly-once), saga compensation rollback | ✅ 16 pytest |
| [`rag-eval-platform`](https://github.com/Sachin-Gupta85/rag-eval-platform) | RAG evaluation: IR ranking metrics (Recall@k, MRR, nDCG) + grounding (faithfulness, context recall) with CIs | ✅ 19 pytest |
| [`llm-observability`](https://github.com/Sachin-Gupta85/llm-observability) | LLM observability: span tracing, token-to-cost accounting, p95/p99 latency percentiles, regression gate | ✅ 26 pytest |
| [`nextjs-enterprise-saas`](https://github.com/Sachin-Gupta85/nextjs-enterprise-saas) | Production enterprise SaaS monorepo: Next.js App Router, Pages Router, React Vite with scalable clean architecture | ✅ Clean |
| [`fullstack-ecommerce-engine`](https://github.com/Sachin-Gupta85/fullstack-ecommerce-engine) | Production Next.js headless e-commerce engine with cart, checkout, and inventory workflows | ✅ Clean |
| [`dsa-master-suite`](https://github.com/Sachin-Gupta85/dsa-master-suite) | Interactive Data Structures & Algorithms visualizer and practice platform (Vite + TypeScript) | ✅ Clean |
| [`mcp-toolbox-server`](https://github.com/Sachin-Gupta85/mcp-toolbox-server) | MCP (FastMCP) server exposing safe calculator, text transformation, units conversion, and SQLite tools | ✅ 9 pytest |
| [`langgraph-sql-assistant`](https://github.com/Sachin-Gupta85/langgraph-sql-assistant) | LangGraph NL→SQL over SQLite with a read-only safety gate, schema inspector, and self-repair loop | ✅ 8 pytest |
| [`langchain-rag-advanced`](https://github.com/Sachin-Gupta85/langchain-rag-advanced) | Advanced RAG: hybrid BM25 + dense retrieval, Reciprocal Rank Fusion (RRF), source-cited FastAPI service | ✅ 8 pytest |
| [`awesome-ai-evaluations`](https://github.com/Sachin-Gupta85/awesome-ai-evaluations) | Curated comprehensive map of LLM/agent benchmarks, evaluation methodology, statistics, and safety frameworks | 📚 Resource |

---

## 🛠️ Technical Stack & Tooling

<div align="center">

| Layer | Technologies & Tooling |
| :--- | :--- |
| **Core Languages** | `Python 3.10+`, `TypeScript`, `JavaScript`, `Bash / Shell Scripting`, `SQL` |
| **Sandbox & Infrastructure** | `Docker`, `Linux Internals`, `POSIX Sockets`, `Systemd`, `Git`, `GitHub Actions` |
| **Testing & Determinism** | `Pytest`, `Subprocess Sandboxing`, `AST Analysis`, `Regex Parsers`, `Vitest / Jest` |
| **Agent Frameworks & SDKs** | `LangGraph`, `LangChain`, `LiteLLM`, `FastMCP (Model Context Protocol)`, `OpenAI SDK` |
| **Evaluation Toolkits** | `Terminal-Bench 3`, `SWE-bench`, `GAIA Benchmark`, `Promptfoo`, `Inspect AI` |
| **Web & Applications** | `Next.js 14 (App & Pages Router)`, `React 18`, `FastAPI`, `TailwindCSS`, `MongoDB`, `Express` |

</div>

---

## 🏆 GitHub Official Achievements & Badges

<div align="center">
  <p>Verified profile milestones and developer badges earned across benchmark and infrastructure repositories.</p>

  <a href="https://github.com/Sachin-Gupta85?tab=achievements">
    <img src="https://raw.githubusercontent.com/Schweinepriester/github-profile-achievements/main/images/tiers/pull-shark-silver.png" alt="Pull Shark Silver" width="105px" style="margin: 0 8px;" />
  </a>
  <a href="https://github.com/Sachin-Gupta85?tab=achievements">
    <img src="https://raw.githubusercontent.com/Schweinepriester/github-profile-achievements/main/images/quickdraw-default.png" alt="Quickdraw" width="105px" style="margin: 0 8px;" />
  </a>
  <a href="https://github.com/Sachin-Gupta85?tab=achievements">
    <img src="https://raw.githubusercontent.com/Schweinepriester/github-profile-achievements/main/images/yolo-default.png" alt="YOLO" width="105px" style="margin: 0 8px;" />
  </a>
  <a href="https://github.com/Sachin-Gupta85?tab=achievements">
    <img src="https://raw.githubusercontent.com/Schweinepriester/github-profile-achievements/main/images/tiers/galaxy-brain-silver.png" alt="Galaxy Brain Silver" width="105px" style="margin: 0 8px;" />
  </a>
  <a href="https://github.com/Sachin-Gupta85?tab=achievements">
    <img src="https://raw.githubusercontent.com/Schweinepriester/github-profile-achievements/main/images/tiers/pair-extraordinaire-bronze.png" alt="Pair Extraordinaire" width="105px" style="margin: 0 8px;" />
  </a>

  <br /><br />

| Badge | Level / Multiplier | Requirement Satisfied | Status |
| :---: | :---: | :--- | :---: |
| 🦈 **Pull Shark** | **Silver (x2)** | 16 merged pull requests into default branches | ![Earned](https://img.shields.io/badge/Status-UNLOCKED-success?style=flat-square&logo=github) |
| ⚡ **Quickdraw** | **Unlocked** | Issue/PR closed within 5 minutes of opening | ![Earned](https://img.shields.io/badge/Status-UNLOCKED-success?style=flat-square&logo=github) |
| 🪂 **YOLO** | **Unlocked** | Pull request merged directly without review block | ![Earned](https://img.shields.io/badge/Status-UNLOCKED-success?style=flat-square&logo=github) |
| 🧠 **Galaxy Brain** | **Silver (x2)** | 8 accepted Q&A answers in public discussions | ![Earned](https://img.shields.io/badge/Status-UNLOCKED-success?style=flat-square&logo=github) |
| 👥 **Pair Extraordinaire** | **Bronze (x1)** | Merged co-authored commits via pull requests | ![Earned](https://img.shields.io/badge/Status-UNLOCKED-success?style=flat-square&logo=github) |

  <p>👉 <em>Inspect live verification badges on <a href="https://github.com/Sachin-Gupta85?tab=achievements"><strong>github.com/Sachin-Gupta85?tab=achievements</strong></a></em></p>
</div>

---

## 📈 GitHub Telemetry & Activity Stats

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=Sachin-Gupta85&theme=tokyonight&no-frame=true&margin-w=12&row=1&column=6" alt="GitHub Trophies" width="100%" />
  <br /><br />
  <img src="https://github-readme-stats.vercel.app/api?username=Sachin-Gupta85&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="Sachin's GitHub Stats" width="48%" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Sachin-Gupta85&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" width="48%" />
</div>

---

## 📬 Contact & Engagements

- 💼 **Available for AI Evaluation Specialist, Benchmark Authoring, and LLM Platform contracts.**
- 🎯 **Platforms:** Mercor, Turing, Scale AI, and frontier AI research labs.
- ✉️ **Direct Email:** **[saching852002@gmail.com](mailto:saching852002@gmail.com)**
- 🔗 **LinkedIn:** **[linkedin.com/in/saching85](https://www.linkedin.com/in/saching85/)**
- 🌐 **GitHub:** **[github.com/Sachin-Gupta85](https://github.com/Sachin-Gupta85)**

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1,6,11,20&height=100&section=footer" width="100%" />
</div>
