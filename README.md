<!-- Header Section -->
<p align="center">
  <a href="https://linkedin.com/in/wisrovi-rodriguez"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://orcid.org/0009-0005-0710-1861"><img src="https://img.shields.io/badge/ORCID-0009--0005--0710--1861-A6CE39?style=for-the-badge&logo=orcid&logoColor=white" alt="ORCID" /></a>
  <a href="https://wisrovi.dev"><img src="https://img.shields.io/badge/Portfolio-wisrovi.dev-111827?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Portfolio" /></a>
  <a href="https://pypi.org/user/wisrovi/"><img src="https://img.shields.io/badge/PyPI-23+_Packages-3775A9?style=for-the-badge&logo=pypi&logoColor=white" alt="PyPI" /></a>
  <a href="https://hub.docker.com/u/wisrovi"><img src="https://img.shields.io/badge/DockerHub-wisrovi-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="DockerHub" /></a>
</p>

<h1 align="center">William Steve Rodriguez Villamizar (wisrovi)</h1>
<h3 align="center">Principal AI Engineer & Applied AI Solutions Architect | Scientific Researcher</h3>

<p align="center">
  <b>Bridging mission-critical production engineering and cutting-edge Artificial Intelligence research. Architect of distributed MLOps clusters, Model Context Protocol (MCP) agentic workflows, and author of 26 peer-reviewed scientific preprints. Based in Badajoz, Spain.</b>
</p>

<p align="center">
  🌐 <b>Official Research & Software Portal: <a href="https://wisrovi.dev">wisrovi.dev</a></b> | 🆔 <b>ORCID ID: <a href="https://orcid.org/0009-0005-0710-1861">0009-0005-0710-1861</a></b>
</p>

---

## 💡 Executive Pitch: Engineering Resilient Ecosystems & Advancing AI Frontiers

In enterprise AI and scientific computing, the critical bottleneck is neither model size nor simple prompting—it is **architectural integrity, statistical safety, and production resilience**.

My work operates at the exact intersection of **hardcore systems engineering** and **rigorous scientific research**:
* **On the Engineering Side**: I engineer distributed, multi-node MLOps platforms, fault-isolated container executors (the Invoker-Executor pattern), asynchronous task routing with Redis priority queues, and maintain **23+ published Python packages on PyPI (37 total ecosystem modules)** coordinated via [`w-cli`](https://github.com/wisrovi/w-cli).
* **On the Scientific Side**: I conduct applied and fundamental research in **Quantitative Explainable AI (XAI)**, **Conformal Prediction**, **In-Training Causal Saliency Regularization**, and **Formal Verification (LTL Model Checking)** for autonomous multi-agent networks.

---

## 🔬 Scientific Research & Peer-Reviewed Preprints (Zenodo / CERN)

Lead investigator of the **wisrovi-suit AI Research Initiative**. All 26 publications feature open reproducible code, mathematical formalization, bootstrap statistical bounds, and official DOIs:

```mermaid
flowchart LR
    A["Cluster Telemetry & Workflows"] --> B["Quantitative XAI & Causal Saliency"]
    B --> C["Safety & Conformal Prediction"]
    C --> D["Formal Verification (LTL/MCP)"]
    D --> E["Autonomous Auditing Gate"]
    
    style A fill:#1e293b,color:#fff,stroke:#38bdf8,stroke-width:2px
    style B fill:#1e293b,color:#fff,stroke:#818cf8,stroke-width:2px
    style C fill:#1e293b,color:#fff,stroke:#34d399,stroke-width:2px
    style D fill:#1e293b,color:#fff,stroke:#fbbf24,stroke-width:2px
    style E fill:#1e293b,color:#fff,stroke:#f87171,stroke-width:2px
```

### 🌟 Featured Research Contributions (Featured in ORCID):
1. **Causal Saliency Regularization (CSR)**: Mitigating Clever Hans Artifacts in Deep Object Detectors via In-Training Explainability Penalties — [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22716676.svg)](https://doi.org/10.5281/zenodo.22716676)
2. **Conformal Prediction & Epistemic Uncertainty Decomposition**: Finite-sample coverage guarantees for safety-critical edge vision under representation-level domain shift — [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22716681.svg)](https://doi.org/10.5281/zenodo.22716681)
3. **Formal Verification of Agentic MLOps Workflows**: Model Checking and Liveness Guarantees in Distributed Model Context Protocol (MCP) Workflows — [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22716667.svg)](https://doi.org/10.5281/zenodo.22716667)
4. **Self-Healing Distributed MLOps**: Autonomous Fault Detection, Node Eviction, and Resilient State Reconciliation in Heterogeneous GPU Clusters — [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22716656.svg)](https://doi.org/10.5281/zenodo.22716656)
5. **Zero-Shot Diffusion Purification**: Stochastic Denoising Defense for YOLO Detectors against Transferable Adversarial Attacks — [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22716695.svg)](https://doi.org/10.5281/zenodo.22716695)

*Explore all 26 manuscripts, datasets, and BibTeX citations at [ORCID Record 0009-0005-0710-1861](https://orcid.org/0009-0005-0710-1861).*

---

## 🌟 Flagship Industrial Platform: NeuralForge AI (Distributed MLOps Cluster)

**[NeuralForge AI (wyoloservice2)](https://github.com/wisrovi/wyoloservice2_production)** is an enterprise-grade distributed hyperparameter optimization and computer vision training platform:

* **API Gateway & Monitoring UI (`NeuralForgeAI` / `:23442`)**: React 19 Single Page Application + FastAPI backend managing studies, datasets, and queue telemetry.
* **Datastore Backbone (`wyoloservice2_control_server`)**: Centralized PostgreSQL, Redis queue manager, MinIO S3 object storage, and MLflow server.
* **Evolutionary Optimization Engine (`wyoloservice2_manager`)**: Distributed Optuna genetic loop (TPESampler) proposing parameter trials.
* **Hardware Quota Daemon (`wyoloservice2_invoker`)**: GPU host agent managing VRAM quotas, CIFS mounts, and launching isolated ephemeral Docker execution containers.
* **Ephemeral Training Engine (`wyoloservice2_worker`)**: Dockerized runtime executing the 22-step post-train forensic pipeline (`wpipe`), XAI heatmaps, noise injection, and automated LLM report synthesis.
* **Strict Multi-Queue Priority Routing**: `private_queue (worker_*) > gpus_high > gpus_medium > gpus_low`.

---

## 🌌 The wisrovi SUITE — 23 Official PyPI Packages (Binary Universe Architecture)

Structured as a **Binary Universe**: the Macro Core Python/MLOps Solar System around central sun `wpipe`, and the Micro Constellation of 6 FastMCP servers for autonomous LLM agents (Claude, Antigravity, Cursor).

```mermaid
flowchart TD
    subgraph Macro_System ["🌌 Macro Solar System: Python & MLOps Infrastructure"]
        Sun["☀️ wpipe (Central Sun)<br/>WAL Engine · GIL Bypass · DAG Checkpoints"]
        
        subgraph Orbit1 ["🪐 Orbit 1: Core Extensions & High Throughput"]
            wkafka["wkafka<br/>Reactive Streaming"]
            wredis["wredis<br/>Distributed Cache & Locks"]
            wdecorators["wdecorators<br/>Resilience & Telemetry"]
            wpipesteps["wpipe-steps<br/>Modular Step Catalog"]
        end
        
        subgraph Orbit2 ["🪐 Orbit 2: Enterprise Persistence & Security"]
            wsqlite["wsqlite<br/>WAL TableSync ORM"]
            wpostgresql["wpostgresql<br/>ACID Pooler"]
            wFabricSecurity["wFabricSecurity<br/>ECDSA Zero Trust"]
            wmongo["wmongo<br/>Reactive ODM"]
            wpipeplugins["wpipe-plugins<br/>Plugin Framework"]
            wutils["wutils<br/>Schedulers & Cron"]
        end
        
        subgraph Orbit3 ["🪐 Orbit 3: Distributed MLOps & Big Data"]
            wyolo["wyolo<br/>YOLO Training Wrapper"]
            wcontainer["wcontainer<br/>Docker & GPU Governor"]
            wclickhouse["wclickhouse<br/>Columnar OLAP"]
            wauth["wauth<br/>Hardware Crypt Vault"]
            wisrovipython["wisrovi-python<br/>Core Foundations"]
            processaudio["ProcessAudio<br/>DSP Mel Transformers"]
        end
        
        Sun --> Orbit1
        Sun --> Orbit2
        Sun --> Orbit3
    end

    subgraph Micro_Constellation ["✨ Micro Constellation: FastMCP Agentic Hub"]
        LLM["🤖 Autonomous AI Agents<br/>(Claude · Antigravity · Cursor)"]
        
        m_wpipe["wpipe-mcp"]
        m_wyolo["wyoloservice-mcp"]
        m_wredis["wredis-mcp"]
        m_wsqlite["wsqlite-mcp"]
        m_wpostgres["wpostgresql-mcp"]
        m_wkafka["wkafka-mcp"]
        
        LLM --> m_wpipe
        LLM --> m_wyolo
        LLM --> m_wredis
        LLM --> m_wsqlite
        LLM --> m_wpostgres
        LLM --> m_wkafka
    end

    Sun -.->|Agentic Orchestration| LLM

    style Sun fill:#1e293b,color:#fff,stroke:#f59e0b,stroke-width:3px
    style LLM fill:#1e293b,color:#fff,stroke:#a855f7,stroke-width:3px
    style Macro_System fill:#0f172a,color:#e2e8f0,stroke:#3b82f6,stroke-width:1px
    style Micro_Constellation fill:#0f172a,color:#e2e8f0,stroke:#8b5cf6,stroke-width:1px
    style Orbit1 fill:#1e293b,color:#fff,stroke:#38bdf8,stroke-width:1px
    style Orbit2 fill:#1e293b,color:#fff,stroke:#34d399,stroke-width:1px
    style Orbit3 fill:#1e293b,color:#fff,stroke:#f43f5e,stroke-width:1px
```

### 🚀 Featured PyPI Flagships (Most Downloaded & Core Orbits)

Rather than cluttering this overview with all 23 packages, here are the primary workhorses driving production traffic:

| Package | Orbit / Role | Monthly Ingestion | Live PyPI Telemetry | Technical Differentiator |
| :--- | :--- | :---: | :---: | :--- |
| **[`wpipe`](https://github.com/wisrovi/wpipe)** | **Central Sun: Core Engine** | Core Sun | [![PyPI](https://img.shields.io/pypi/v/wpipe?color=3b82f6)](https://pypi.org/project/wpipe/) | In-process DAG orchestrator, zero-infra, SQLite WAL checkpoints, GIL bypass. |
| **[`wkafka`](https://github.com/wisrovi/wkafka)** | **Orbit 1: Event Streaming** | **~1,558 / mo** | [![Downloads](https://img.shields.io/pypi/dm/wkafka?color=10b981)](https://pypi.org/project/wkafka/) | Reactive Kafka wrapper, declarative `@kafka.consumer` decorators, auto-reconnect. |
| **[`wredis`](https://github.com/wisrovi/wredis)** | **Orbit 1: Cache & Atomicity** | **~798 / mo** | [![Downloads](https://img.shields.io/pypi/dm/wredis?color=10b981)](https://pypi.org/project/wredis/) | Sub-millisecond async Redis caching, atomic distributed locks, token-bucket limiter. |
| **[`wdecorators`](https://github.com/wisrovi/wdecorators)** | **Orbit 1: Resilience** | **~655 / mo** | [![Downloads](https://img.shields.io/pypi/dm/wdecorators?color=10b981)](https://pypi.org/project/wdecorators/) | Zero-overhead jittered backoff, microsecond latency profiling, auto-telemetry. |
| **[`wpipe-steps`](https://github.com/wisrovi/wpipe-steps)** | **Orbit 1: Catalog** | **~184 / mo** | [![Downloads](https://img.shields.io/pypi/dm/wpipe-steps?color=10b981)](https://pypi.org/project/wpipe-steps/) | Production catalog of 196+ standardized, pluggable ETL steps for `wpipe`. |
| **[`wsqlite`](https://github.com/wisrovi/wsqlite)** | **Orbit 2: ACID Persistence** | Enterprise | [![PyPI](https://img.shields.io/pypi/v/wsqlite?color=3b82f6)](https://pypi.org/project/wsqlite/) | Enterprise SQLite with TableSync reactive migrations and Pydantic v2 ORM. |
| **[`wFabricSecurity`](https://github.com/wisrovi/wFabricSecurity)** | **Orbit 2: Zero Trust** | Enterprise | [![PyPI](https://img.shields.io/pypi/v/wfabricsecurity?color=3b82f6)](https://pypi.org/project/wfabricsecurity/) | Hardware-grade zero trust, ECDSA P-256 signatures, and SHA-256 payload proofs. |

<p align="center">
  📦 <b>Explore all 23 official ecosystem packages and MCP tools on <a href="https://pypi.org/user/wisrovi/">PyPI Profile (@wisrovi)</a> and the interactive portal at <a href="https://wisrovi.dev">wisrovi.dev</a>.</b>
</p>

---

## 🛠️ Technical Competencies & Toolchain

<table>
  <tr>
    <td valign="top" width="25%"><b>🧠 Agentic AI & LLMs</b></td>
    <td valign="top" width="75%">Model Context Protocol (MCP), LangGraph, LangChain, Agentic RAG, Semantic Caching, Local LLM Inference (vLLM, Ollama), Groundedness Auditing</td>
  </tr>
  <tr>
    <td valign="top" width="25%"><b>🤖 Vision & Mathematics</b></td>
    <td valign="top" width="75%">YOLO (v8, v11, v26), RT-DETR, PyTorch, Causal Inference, Conformal Prediction, Formal Verification (LTL Model Checking), Grad-CAM/Eigen-CAM, Itô SDEs</td>
  </tr>
  <tr>
    <td valign="top" width="25%"><b>⚡ Programming & Core</b></td>
    <td valign="top" width="75%"><b>Python (Primary Engineering Weapon)</b>, Bash/Shell, C/C++, SQL, TypeScript/JavaScript (ES6+)</td>
  </tr>
  <tr>
    <td valign="top" width="25%"><b>🗄️ Storage & Datastores</b></td>
    <td valign="top" width="75%">PostgreSQL, Redis, MinIO S3, SQLite (WAL mode), ClickHouse, MongoDB, PgVector, Milvus</td>
  </tr>
  <tr>
    <td valign="top" width="25%"><b>🐳 MLOps & Infrastructure</b></td>
    <td valign="top" width="75%">Docker, Celery, MLflow, Optuna, FastMCP, NATS, Linux Kernel Tuning, NVIDIA Container Toolkit, CIFS/Samba, Git CI/CD</td>
  </tr>
</table>

---

## 🎮 Interactive Showcase: Wisrovi Legacy

* **[Wisrovi Legacy (Live Game)](https://wisrovi.github.io)**: A procedural 3D driving RPG built with Vanilla JavaScript and WebGL/Three.js showcasing the libraries and distributed MLOps architecture in an interactive virtual science campus.

---

## 🎯 Doctoral Research Agenda & Theoretical Pillars

As an aspiring Ph.D. candidate, my doctoral research focuses on **Autonomous Verification, Causal Explainability, and Statistical Safety in Distributed Vision Architectures**. I investigate three foundational scientific questions:

1. **Causal Saliency & Shortcut Mitigation:** How can we mathematically penalize non-causal representation shortcuts during gradient descent without sacrificing real-time detection throughput ($mAP_{50}$ vs. Deletion/Insertion AUC Pareto optimality)?
2. **Conformal Prediction under Dynamic Domain Shift:** Establishing finite-sample, distribution-free coverage bounds for deep detectors operating under heavy sensor degradation and non-stationary edge environments.
3. **Formal Verification of Distributed Agentic Workflows:** Synthesizing runtime verification monitors and model checkers based on Linear Temporal Logic (LTL) to guarantee safety, dead-lock freedom, and liveness in autonomous multi-agent tool execution (Model Context Protocol).

---

## 🎓 Academic Credentials & Professional Memberships

* **M.Sc. in Artificial Intelligence** — Universidad Internacional de Valencia (VIU), Spain (2023–2024).
* **B.Sc. in Electronic Engineering** — Universidad de Investigación y Desarrollo (UDI), Colombia (2010–2016).
* **Professional Member** — IEEE Computer Society (Member #9983421).
* **Principal Investigator & Grantee** — wisrovi-suit AI Research Initiative (Badajoz, Extremadura, Spain).

---

<p align="center">
  <i>"Rigorous systems engineering in production; uncompromising mathematical rigor in research."</i>
</p>
<p align="center">
  <sub>© 2026 William Steve Rodriguez Villamizar (wisrovi). Distributed under the MIT License. Open for academic research collaborations.</sub>
</p>
