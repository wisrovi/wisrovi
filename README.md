<!-- Header Section -->
<p align="center">
  <a href="https://linkedin.com/in/wisrovi-rodriguez"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://orcid.org/0009-0005-0710-1861"><img src="https://img.shields.io/badge/ORCID-0009--0005--0710--1861-A6CE39?style=for-the-badge&logo=orcid&logoColor=white" alt="ORCID" /></a>
  <a href="https://wisrovi.dev"><img src="https://img.shields.io/badge/Portfolio-wisrovi.dev-111827?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Portfolio" /></a>
  <a href="https://pypi.org/user/wisrovi/"><img src="https://img.shields.io/badge/PyPI-26+_Packages-3775A9?style=for-the-badge&logo=pypi&logoColor=white" alt="PyPI" /></a>
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
* **On the Engineering Side**: I engineer distributed, multi-node MLOps platforms, fault-isolated container executors (the Invoker-Executor pattern), asynchronous task routing with Redis priority queues, and maintain **26+ published Python packages** on PyPI.
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

## 🧱 The wisrovi SUITE — 26+ Published Python Packages

| Package | Category | PyPI Status | Technical Highlight |
| :--- | :--- | :--- | :--- |
| **`wpipe`** | Pipeline Engine | [![PyPI](https://img.shields.io/pypi/v/wpipe)](https://pypi.org/project/wpipe/) | WAL SQLite state storage, GIL bypass, dynamic DAG checkpointing. |
| **`wpipe-mcp`** | Agentic AI | [![PyPI](https://img.shields.io/pypi/v/wpipe-mcp)](https://pypi.org/project/wpipe-mcp/) | FastMCP tool server allowing LLMs to safely build, audit, and run pipelines. |
| **`wsqlite`** | Database ORM | [![PyPI](https://img.shields.io/pypi/v/wsqlite)](https://pypi.org/project/wsqlite/) | TableSync schema generator, Pydantic v2 serialization, soft delete mixins. |
| **`wredis`** | Caching / Queues | [![PyPI](https://img.shields.io/pypi/v/wredis)](https://pypi.org/project/wredis/) | Sync/async Redis pooling, cache decorators, distributed token-bucket rate limiters. |
| **`wauth`** | Cryptography | [![PyPI](https://img.shields.io/pypi/v/wauth)](https://pypi.org/project/wauth/) | Machine-salted hardware fingerprint encryption vault (Fernet AES-256). |
| **`wFabricSecurity`** | Zero Trust | [![PyPI](https://img.shields.io/pypi/v/wfabricsecurity)](https://pypi.org/project/wfabricsecurity/) | ECDSA P-256 digital signature validation and SHA-256 code integrity verifiers. |
| **`wyolo`** | Vision MLOps | [![PyPI](https://img.shields.io/pypi/v/wyolo)](https://pypi.org/project/wyolo/) | Automated MLflow & S3 lifecycle wrapper for YOLO and RT-DETR architectures. |
| **`ProcessAudio`** | Signal Processing | [![PyPI](https://img.shields.io/pypi/v/ProcessAudio)](https://pypi.org/project/ProcessAudio/) | Scikit-learn feature transformers for audio spectrograms and data augmentation. |
| **`wticket`** | Enterprise Apps | [![PyPI](https://img.shields.io/pypi/v/wticket)](https://pypi.org/project/wticket/) | Dynamic SLA helpdesk engine with client portal APIs. Live demo: [wticket.wisrovi.dev](https://wticket.wisrovi.dev/). |

*Explore the full catalog of packages on [PyPI (wisrovi)](https://pypi.org/user/wisrovi/) and source repositories on [GitHub](https://github.com/wisrovi).*

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

* **M.Sc. in Artificial Intelligence** — Universidad Internacional de Valencia (VIU), Spain (*Honors thesis track*).
* **B.Sc. in Electronic Engineering** — Universidad de Investigación y Desarrollo (UDI), Colombia (*Magna cum laude project*).
* **Professional Member** — IEEE Computer Society (Member #9983421).
* **Principal Investigator & Grantee** — wisrovi-suit AI Research Initiative (Badajoz, Extremadura, Spain).

---

<p align="center">
  <i>"Rigorous systems engineering in production; uncompromising mathematical rigor in research."</i>
</p>
<p align="center">
  <sub>© 2026 William Steve Rodriguez Villamizar (wisrovi). Distributed under the MIT License. Open for academic research collaborations.</sub>
</p>
