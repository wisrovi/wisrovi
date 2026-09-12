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

| Package | Category / Orbit | PyPI Status | Technical Highlight |
| :--- | :--- | :--- | :--- |
| **`wpipe`** | Macro Sun: Pipeline Engine | [![PyPI](https://img.shields.io/pypi/v/wpipe)](https://pypi.org/project/wpipe/) | WAL SQLite state storage, GIL bypass, dynamic DAG checkpointing. |
| **`wkafka`** | Macro Orbit 1: Streaming | [![PyPI](https://img.shields.io/pypi/v/wkafka)](https://pypi.org/project/wkafka/) | Reactive Apache Kafka abstraction (~1,558/mo), declarative retry decorators. |
| **`wredis`** | Macro Orbit 1: Cache & Locks | [![PyPI](https://img.shields.io/pypi/v/wredis)](https://pypi.org/project/wredis/) | Ultralong distributed caching (~798/mo), atomic locks, token-bucket limiter. |
| **`wdecorators`** | Macro Orbit 1: Resilience | [![PyPI](https://img.shields.io/pypi/v/wdecorators)](https://pypi.org/project/wdecorators/) | Exponential retries with jitter (~655/mo), latency profiling, and telemetry. |
| **`wpipe-steps`** | Macro Orbit 1: Modular Steps | [![PyPI](https://img.shields.io/pypi/v/wpipe-steps)](https://pypi.org/project/wpipe-steps/) | Modular, production-ready standardized pipeline step catalog (~184/mo). |
| **`wsqlite`** | Macro Orbit 2: Database | [![PyPI](https://img.shields.io/pypi/v/wsqlite)](https://pypi.org/project/wsqlite/) | TableSync reactive schema generator, multithread WAL mode, Pydantic v2. |
| **`wpostgresql`** | Macro Orbit 2: Database | [![PyPI](https://img.shields.io/pypi/v/wpostgresql)](https://pypi.org/project/wpostgresql/) | High-concurrency ACID transactional pooler and ORM mapping for PostgreSQL. |
| **`wFabricSecurity`** | Macro Orbit 2: Zero Trust | [![PyPI](https://img.shields.io/pypi/v/wfabricsecurity)](https://pypi.org/project/wfabricsecurity/) | Zero Trust security for Hyperledger Fabric (ECDSA P-256 and SHA-256 integrity). |
| **`wmongo`** | Macro Orbit 2: Database | [![PyPI](https://img.shields.io/pypi/v/wmongo)](https://pypi.org/project/wmongo/) | Reactive MongoDB ODM with Pydantic models and automatic Redis caching. |
| **`wpipe-plugins`** | Macro Orbit 2: Extensions | [![PyPI](https://img.shields.io/pypi/v/wpipe-plugins)](https://pypi.org/project/wpipe-plugins/) | Dynamic community extension framework for modular wpipe pipelines. |
| **`wutils`** | Macro Orbit 2: Utilities | [![PyPI](https://img.shields.io/pypi/v/wutils)](https://pypi.org/project/wutils/) | Schedulers, safe cron expression parsing, and data format validation. |
| **`wyolo`** | Macro Orbit 3: Vision MLOps | [![PyPI](https://img.shields.io/pypi/v/wyolo)](https://pypi.org/project/wyolo/) | Automated YOLOv8/v11/v26 wrapper with MLflow telemetry and MinIO S3 sync. |
| **`wcontainer`** | Macro Orbit 3: Docker Engine | [![PyPI](https://img.shields.io/pypi/v/wcontainer)](https://pypi.org/project/wcontainer/) | Docker SDK governor, dynamic GPU VRAM/CPU quotas, and container lifecycle. |
| **`wclickhouse`** | Macro Orbit 3: Big Data | [![PyPI](https://img.shields.io/pypi/v/wclickhouse)](https://pypi.org/project/wclickhouse/) | High-throughput columnar OLAP analytics ORM for ClickHouse batches. |
| **`wauth`** | Macro Orbit 3: Cryptography | [![PyPI](https://img.shields.io/pypi/v/wauth)](https://pypi.org/project/wauth/) | Machine-salted hardware fingerprint encryption vault (Fernet AES-256). |
| **`wisrovi-python`** | Macro Orbit 3: Foundational | [![PyPI](https://img.shields.io/pypi/v/wisrovi-python)](https://pypi.org/project/wisrovi-python/) | Foundational shared types, algorithms, and mathematical utilities of the suite. |
| **`ProcessAudio`** | Macro Orbit 3: Signal DSP | [![PyPI](https://img.shields.io/pypi/v/ProcessAudio)](https://pypi.org/project/ProcessAudio/) | Scikit-learn transformers for Mel-spectrograms, MFCC, and audio DSP augmentation. |
| **`wpipe-mcp`** | Micro MCP Constellation | [![PyPI](https://img.shields.io/pypi/v/wpipe-mcp)](https://pypi.org/project/wpipe-mcp/) | FastMCP server for pipeline topology, context verification, and dry-runs. |
| **`wyoloservice-mcp`** | Micro MCP Constellation | [![PyPI](https://img.shields.io/pypi/v/wyoloservice-mcp)](https://pypi.org/project/wyoloservice-mcp/) | FastMCP agentic tools for remote GPU cluster orchestration & Optuna sweeps. |
| **`wredis-mcp`** | Micro MCP Constellation | [![PyPI](https://img.shields.io/pypi/v/wredis-mcp)](https://pypi.org/project/wredis-mcp/) | FastMCP safe key inspection, datastores telemetry, and memory profiling. |
| **`wsqlite-mcp`** | Micro MCP Constellation | [![PyPI](https://img.shields.io/pypi/v/wsqlite-mcp)](https://pypi.org/project/wsqlite-mcp/) | FastMCP safe parameterized querying and SQLite schema extraction. |
| **`wpostgresql-mcp`** | Micro MCP Constellation | [![PyPI](https://img.shields.io/pypi/v/wpostgresql-mcp)](https://pypi.org/project/wpostgresql-mcp/) | FastMCP relational database inspection and transaction monitoring. |
| **`wkafka-mcp`** | Micro MCP Constellation | [![PyPI](https://img.shields.io/pypi/v/wkafka-mcp)](https://pypi.org/project/wkafka-mcp/) | FastMCP topic telemetry, consumer group lag monitoring, and event streaming. |

*Explore all 23 official packages on [PyPI (wisrovi)](https://pypi.org/user/wisrovi/) and source code on [GitHub](https://github.com/wisrovi).*

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
