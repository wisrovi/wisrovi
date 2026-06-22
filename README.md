<!-- Header Section -->
<p align="center">
  <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="LinkedIn" width="24" height="24" /> 
  <a href="https://linkedin.com/in/wisrovi-rodriguez"><b>LinkedIn</b></a> | 
  <a href="https://wisrovi.dev"><b>Portfolio</b></a> | 
  <a href="mailto:wisrovi.rodriguez@gmail.com"><b>Email Me</b></a>
</p>

<h1 align="center">William Rodriguez (wisrovi)</h1>
<h3 align="center">AI Solutions Architect & Principal Software Engineer</h3>

<p align="center">
  <a href="https://github.com/ryo-ma/github-profile-trophy">
    <img src="https://github-profile-trophy.vercel.app/?username=wisrovi&theme=onedark&column=7" alt="wisrovi trophies" />
  </a>
</p>

<p align="center">
  <b>Python is my peak weapon. I engineer highly-resilient, production-ready AI agents, MLOps platforms, and custom software infrastructure. Based in Badajoz, Spain.</b>
</p>

<p align="center">
  🌐 <b>Official Website & Interactive Showcase: <a href="https://wisrovi.dev">wisrovi.dev</a></b>
</p>

---

## 💡 Executive Pitch: I Don't Just Write Code; I Engineer Ecosystems

In modern engineering, the bottleneck is rarely writing code—it is **resiliency, scalability, and design integrity**. 

While many build simple AI wrappers, my primary focus is designing **high-availability systems where Generative AI, Computer Vision, and modular infrastructure converge** to solve complex enterprise problems. 

By leveraging **Python** as my supreme engineering backbone, I create custom frameworks, distributed MLOps clusters, and multi-agent state machines designed to survive in high-concurrency production workloads.

---

## 🧠 Core Competencies

### 1. 🤖 Generative AI & Agentic Architectures
I design next-generation cognitive systems that move past simple prompt engineering into complex, stateful reasoning loops.
*   **Stateful Agent Orchestration**: Building multi-agent systems using **LangGraph** and **LangChain** to orchestrate structured, reliable agent behaviors.
*   **RAG (Retrieval-Augmented Generation)**: Engineering advanced semantic search and query expansion pipelines, utilizing vector embeddings and vector databases (Milvus, PgVector) to inject contextual accuracy.
*   **Generative AI & LLMs**: Implementing LLM integration patterns, reasoning validation, fine-tuning structures, and safety/security filters.

### 2. ⚡ Python Infrastructure Engineering (The wisrovi SUITE)
I believe in writing code that other developers rely on. To solve common bottlenecks in database operations, caching, and pipeline orchestration, I built a catalog of **26+ custom Python libraries**:
*   **Orchestration (`wpipe`)**: A lightweight Python pipeline executor featuring WAL-mode SQLite state storage, GIL bypass, DAG scheduling, and dynamic checkpoints.
*   **ORM Systems (`wsqlite`, `wredis`, `wclickhouse`)**: Custom wrappers resolving database concurrency, soft deletions, and bulk insertions utilizing Pydantic v2 schemas.
*   **Zero Trust Security (`wauth`, `wFabricSecurity`)**: Cryptographic vaults tying encryption to salted machine hardware signatures and securing distributed networks.

### 3. 🔬 Computer Vision & MLOps
Scaling training campaigns from a single workstation to distributed clusters.
*   **MLOps Automation**: Complete training lifecycle management of YOLO and RT-DETR models.
*   **Distributed Compute**: Celery-based worker structures mapping and utilizing GPU topologies, autobatching weights based on VRAM capacity, and tracking runs via MLflow.

---

## 🌟 Flagship Project: NeuralForge AI (Distributed YOLO Cluster)

**[NeuralForge AI](https://github.com/wisrovi/train_service2)** is the ultimate demonstration of my engineering philosophy. It is a distributed hyperparameter optimization and training ecosystem built entirely on top of the **wisrovi SUITE**.

*   **Resilient Scheduling**: Uses the **`wpipe`** DAG engine to manage states, training retries, and task checkpoints.
*   **MLOps Lifecycle**: Employs **`wyolo`** to execute training loops, auto-configure datasets (via S3/MinIO), and log telemetry directly into MLflow.
*   **Distributed Scaling**: Celery queue architectures (Invoker/Executor pattern) and **Optuna** studies running across multiple GPU-accelerated Docker nodes.

---

## 🧱 The wisrovi SUITE — Main Index

| Component | Category | Registry / Status | Focus & Key Technical Specs |
| :--- | :--- | :--- | :--- |
| **`wpipe`** | Core Engine | [![PyPI Downloads](https://static.pepy.tech/personalized-badge/wpipe?period=total&units=NONE&left_color=BLACK&right_color=GREEN&left_text=downloads)](https://pepy.tech/projects/wpipe) | WAL SQLite state storage, GIL bypass, thread/process parallel setups. |
| **`wpipe-mcp`** | Generative AI | `Internal` | Model Context Protocol (MCP) server letting LLMs program and deploy pipelines. |
| **`wsqlite`** | Database ORM | [![PyPI Downloads](https://static.pepy.tech/personalized-badge/wsqlite?period=total&units=NONE&left_color=BLACK&right_color=GREEN&left_text=downloads)](https://pepy.tech/projects/wsqlite) | TableSync migration generator, soft deletion query filters, connection pooling. |
| **`wauth`** | Security | [![PyPI Downloads](https://static.pepy.tech/personalized-badge/wauth?period=total&units=NONE&left_color=BLACK&right_color=GREEN&left_text=downloads)](https://pepy.tech/projects/wauth) | Secrets vault tied deterministically to machine hardware signatures (Fernet). |
| **`wredis`** | Database ORM | [![PyPI Downloads](https://static.pepy.tech/personalized-badge/wredis?period=total&units=NONE&left_color=BLACK&right_color=GREEN&left_text=downloads)](https://pepy.tech/projects/wredis) | Sync/async Redis integration, cache expiration decorators, rate-limiters. |
| **`wFabricSecurity`**| Security | [![PyPI Downloads](https://static.pepy.tech/personalized-badge/wfabricsecurity?period=total&units=NONE&left_color=BLACK&right_color=GREEN&left_text=downloads)](https://pepy.tech/projects/wfabricsecurity) | Zero Trust security system for Hyperledger Fabric (ECDSA signatures). |
| **`wyolo`** | MLOps | `Development` | MLflow + S3 automation wrapper for YOLO & RT-DETR models. |
| **`ProcessAudio`** | MLOps / Audio | [![PyPI Downloads](https://static.pepy.tech/personalized-badge/ProcessAudio?period=total&units=NONE&left_color=BLACK&right_color=GREEN&left_text=downloads)](https://pepy.tech/projects/ProcessAudio) | Librosa feature extraction & audio data augmentation. |
| **`wticket`** | Support / Helpdesk | [![PyPI Downloads](https://static.pepy.tech/personalized-badge/wticket?period=total&units=NONE&left_color=BLACK&right_color=GREEN&left_text=downloads)](https://pepy.tech/projects/wticket) | Helpdesk manager with dynamic SLAs and client portal APIs. Live demo: [wticket.wisrovi.dev](https://wticket.wisrovi.dev/). |

*Explore all 26+ packages in my [complete library repository](https://github.com/wisrovi/w-cli).*

---

## 🛠️ Technology Stack

<table>
  <tr>
    <td valign="top" width="20%">
      <b>🧠 Generative AI</b>
    </td>
    <td valign="top" width="80%">
      LangGraph, LangChain, RAG, LLM Engineering, Vector Databases (Milvus, PgVector), OpenAI API, HuggingFace
    </td>
  </tr>
  <tr>
    <td valign="top" width="20%">
      <b>🤖 Computer Vision</b>
    </td>
    <td valign="top" width="80%">
      YOLO, RT-DETR, OpenCV, PyTorch, TensorFlow, Scikit-Learn
    </td>
  </tr>
  <tr>
    <td valign="top" width="20%">
      <b>💻 Programming</b>
    </td>
    <td valign="top" width="80%">
      <b>Python (Peak Weapon)</b>, Bash/Shell, C/C++, Java, SQL, JavaScript (ES6)
    </td>
  </tr>
  <tr>
    <td valign="top" width="20%">
      <b>🗄️ Databases</b>
    </td>
    <td valign="top" width="80%">
      SQLite, Redis, ClickHouse, PostgreSQL, MySQL, MariaDB, MongoDB, Elasticsearch, Snowflake
    </td>
  </tr>
  <tr>
    <td valign="top" width="20%">
      <b>🐳 DevOps / Infra</b>
    </td>
    <td valign="top" width="80%">
      Docker, Celery, NATS, Kafka, ZeroMQ, HAProxy, DVC, AWS (S3, AWS API), Git CI/CD
    </td>
  </tr>
</table>

---

## 🎮 Game Development
*   **[Wisrovi Legacy](https://wisrovi.github.io)**: A procedural 3D driving RPG built with Vanilla JS and WebGL/Three.js. Demonstrates my frontend abilities and procedural texture rendering.

---

## 📊 Github Metrics

<p align="center">
  <img align="left" src="https://github-readme-stats.vercel.app/api/top-langs?username=wisrovi&show_icons=true&locale=en&layout=compact&theme=onedark" alt="wisrovi languages" />
  <img align="center" src="https://github-readme-stats.vercel.app/api?username=wisrovi&show_icons=true&locale=en&theme=onedark" alt="wisrovi stats" />
</p>

---

## 📄 Technical Manual: Kubernetes GPU Integration for MLOps Workloads

A comprehensive 22-page technical guide has been compiled and is available as a PDF in this repository:
*   **Location**: [main.pdf](file:///home/william.rodriguez/Documents/w_libraries/wisrovi/main.pdf)
*   **LaTeX Source**: [docs/main.tex](file:///home/william.rodriguez/Documents/w_libraries/wisrovi/docs/main.tex)
*   **Contents**: Detailed architecture diagrams of the `w-libraries` suite, step-by-step installation routines for docker/GPU runtimes, Optuna-Celery configurations, and future roadmaps with LangGraph/RAG integrations.

---

## ☕ Support My Work

If you find my open-source projects or guides helpful, feel free to support my ongoing research:

<p align="left">
  <a href="https://www.buymeacoffee.com/wisrovirod8" target="_blank">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" height="42" style="vertical-align:middle" />
  </a>
  &nbsp;&nbsp;
  <a href="https://ko-fi.com/williamrodriguez" target="_blank">
    <img src="https://cdn.ko-fi.com/cdn/kofi3.png?v=3" alt="Ko-Fi" height="42" style="vertical-align:middle" />
  </a>
</p>

---

<p align="center">
  <i>"I love to research and learn as much as I love chess or my family."</i>
</p>
