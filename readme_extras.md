# Wisrovi Ecosystem & Workspace Developer Guide (readme_extras.md)

This document is a technical reference guide containing a comprehensive mapping of the workspace at `/home/william.rodriguez/Documents/w_libraries`. It details the developer's profile, system architectures, directories, and codebases.

---

## 👤 1. Developer Profile & Engineering Philosophy

*   **Developer**: William Rodriguez (wisrovi / wisrovirod8)
*   **Role**: AI Leader & Solutions Architect at eCaptureDtech (Badajoz, Extremadura, Spain).
*   **Core Languages**: **Python** (supreme professional weapon), Shell/Bash, JavaScript (ES6), SQL, C/C++, Java.
*   **Key Architectures**:
    *   **Generative AI**: LangGraph, LangChain, Retrieval-Augmented Generation (RAG) with Milvus/PgVector, LLM orchestration.
    *   **Computer Vision & MLOps**: YOLO & RT-DETR training pipelines, automated MLflow metric registries, S3 storage integration.
    *   **Systems Concurrency**: Celery distributed worker tasks, Redis broker queues, ZeroMQ TCP/IPC sockets.
    *   **Zero Trust Security**: ECDSA P-256 signatures, SHA-256 code integrity verifications, platform-salted hardware credentials vaults.
*   **QA Standards & Rules**:
    *   Pylint score targets $>9.5/10$.
    *   Bandit static security scanners integrated into pre-commit workflows.
    *   Tests run via `pytest` inside isolated Docker containers (managed by execution bash scripts).
    *   One commit per modified file for Git version control.

---

## 📁 2. Top-Level Workspace Mapping

### A. `imagenesDocker`
*   **Objective**: Comprehensive repository of optimized Docker images and orchestrator compose files categorized by purpose.
*   **Directory Structure**:
    *   `00 docker and nvidia-docker-toolkit install`: Base installers, GPU setups, kind Kubernetes configurations.
    *   `01 databases`: Compose files for Milvus, Oracle, Postgres (v13 & v16.4), MongoDB, MariaDB, MySQL, Redis, and Graylog.
    *   `02 devops`: Advanced container topologies (Doon - Docker-over-Docker, Diun - Docker-in-Docker), queues (Kafka, MQTT, Celery), QA (SonarQube, Uptime Kuma, Heimdall, Homer, Portainer with SSL certs), Nginx load balancing, and Jenkins pipelines.
    *   `03 ArtificalInteligence`: CUDA test beds (PyTorch/Tensorflow with GPU passthroughs), DVC setups, Ollama runners, and agent environments.
    *   `04 cibersecurity`: VPN tools, proxy configurations.
    *   `05 professional`: WordPress + MariaDB stacks, NovoSga queue system, OpenKM ECM systems.
    *   `06 personals` & `07 generals`: Speedtest, Mealie recipes, VS Code server.
    *   `08 projects`: Password generator APIs.
    *   `09 games` & `10 Other`: Retro game servers, experimental environments.

### B. `other/API_face_recognition`
*   **Objective**: REST API for facial recognition secured by JWT and a specialized license controller.
*   **Core Mechanics**:
    *   FastAPI endpoint mapping: `/faces_to_fingerprint` to vectorize image faces.
    *   Uses Swagger UI documentation at `/docs`.
    *   License module tracks byte consumption, expiry dates, and vectorized face limitations (all configurations stored in a local JSON db).
    *   Front-end: UI web page container running alongside the REST container.

### C. `other/analyze-code-quality`
*   **Objective**: Automated Pull Request reviewer structured as a 3-tier microservice architecture.
*   **Sub-Services**:
    *   `github_download` (Port 8033): FastAPI endpoint `POST /api/v1/pr/download-pr-files` downloads repository PR edits as raw ZIP archives.
    *   `python_check` (Port 8032): Batch audits files utilizing Pylint (scoring), Flake8 (style checking), MyPy (types checking), complexity estimators, and secret scans.
    *   `pr_reviewer` (Port 8034): Main orchestration backend. Captures webhook events, triggers files download, runs quality checks, and publishes review comments back to Github PR threads.

### D. `train_service_1` (wyoloservice)
*   **Objective**: Legacy containerized YOLO model training setup.
*   **Mechanics**: Auto-scales swap memory buffers to match physical RAM sizes using `fallocate -l 32G /swapfile` scripts to prevent training processes crash. Downloads and runs `wisrovi/wyoloservice` images.

### E. `train_service2` (NeuralForge AI)
*   **Objective**: Flagship distributed hyperparameter optimization and training cluster.
*   **Sub-components**:
    *   `wyoloservice2_control_server`: FastAPI gateway validating study input configuration YAMLs and posting Celery jobs.
    *   `wyoloservice2_manager`: Celery worker implementing **Optuna** studies. Suggests hyperparameters, pushes task runs to invoker worker queues, and collects metrics.
    *   `wyoloservice2_invoker`: Celery worker listening to GPU-specific queues. Queries PostgreSQL database for current trial variables, runs training runs inside ephemeral executor Docker containers, and registers findings.
    *   `wyoloservice2_production`: Live docker-compose orchestration, PostgreSQL setups, and MLflow servers.

### F. `wisrovi.github.io` (Wisrovi Legacy)
*   **Objective**: A procedural 3D RPG driving game built with Vanilla JavaScript and WebGL (Three.js).
*   **Code Architecture**:
    *   [`js/main.js`](file:///home/william.rodriguez/Documents/w_libraries/wisrovi.github.io/js/main.js): Main game initializer. Configures input listeners, renderer loops, loading/saving states, achievements, and starts the clock.
    *   [`js/game/world.js`](file:///home/william.rodriguez/Documents/w_libraries/wisrovi.github.io/js/game/world.js): Generates the procedural urban layout. Synthesizes buildings with procedural window patterns using HTML canvas textures (`createBuildingTexture`), maps streets and asphalt lines, and registers zones.
    *   [`js/game/player.js`](file:///home/william.rodriguez/Documents/w_libraries/wisrovi.github.io/js/game/player.js): Controls vehicle physics (accel, brake, drift), camera collision mappings, and intersects resource zones.
    *   [`js/game/missions.js`](file:///home/william.rodriguez/Documents/w_libraries/wisrovi.github.io/js/game/missions.js) & [`js/game/achievements.js`](file:///home/william.rodriguez/Documents/w_libraries/wisrovi.github.io/js/game/achievements.js): Quest tracking, objectives validation, and trophy unlock mechanics.
    *   [`js/ui/manager.js`](file:///home/william.rodriguez/Documents/w_libraries/wisrovi.github.io/js/ui/manager.js): Updates glassmorphic DOM elements (inventory grids, mission UI, welcome screens, and market panels).

---

## 🧱 3. The wisrovi-suite Libraries Deep Dive

These packages reside under `/home/william.rodriguez/Documents/w_libraries/w_libraries`.

### 1. `wpipe` (Pipeline Orchestrator)
*   **Module structure**:
    *   `pipe.py` / `pipe_async.py`: Contains `Pipeline` and `PipelineAsync`. Houses variables like `tasks_list`, retry controllers (`max_retries`, `retry_delay`), telemetry variables, and progression trackers.
    *   `components/logic_blocks.py`: Implements logic control flow blocks (`Condition`, `For`, `Parallel`, `Background`).
    *   `checkpoint/`: Serializes execution state variables. Recovers pipelines after process crashes.
    *   `dashboard/`: FastAPI web dashboard running on port 8035.
*   **Performance Optimization**:
    *   Launches with lazy modules loader (`_LAZY_MAP` inside `__init__.py`) to prevent startup latency.
    *   Monkey-patches `wsqlite` connections: Forces `PRAGMA journal_mode=WAL`, `PRAGMA synchronous=OFF`, and high cache sizes using connection locks (`_db_lock`).

### 2. `wsqlite` (Pydantic SQLite ORM)
*   **Module structure**:
    *   `core/repository.py`: Implements `WSQLite` class. Sanitizes input parameters using `validate_identifier` to prevent SQL Injections. Maps `_execute` queries, hook triggers, and soft-delete filters (`IS NULL` checks).
    *   `core/sync.py`: Implements `TableSync`. Traverses Pydantic model fields, maps Python types to SQLite data column definitions, runs schema generation (`create_if_not_exists`), and handles column additions.
    *   `core/pool.py`: Implements connection pool engines (`ConnectionPool`, `AsyncConnectionPool`).
    *   `models.py`: Provides reusable mixins (`TimestampMixin`, `SoftDeleteMixin`, `AuditMixin`).

### 3. `wauth` (Secrets Vault)
*   **Module structure**:
    *   `vault.py`: Declares `SecretModel` (key, value, type, created_at, updated_at, ttl) mapped to a local SQLite database (`~/.wisrovi/wauth.db`).
    *   `core.py`: Houses `CryptoEngine` executing AES-256 encryption via Fernet.
    *   `utils.py`: Derives machine keys dynamically. Reads `/etc/machine-id` (Linux), `csproduct uuid` (Windows), or `IOPlatformUUID` (macOS), hashes the hardware ID string with a local salt, and returns a 32-byte key.
    *   `drivers/local.py`: Evaluates TTLs, deletes keys, and executes secret rotation.

### 4. `wyolo` (YOLO MLOps Framework)
*   **Module structure**:
    *   `trainer/trainer_wrapper.py`: Implements `TrainerWrapper` extending `Elemental` and `Mlflow_setup`. Hook handlers (`on_train_start`, `on_train_end`) read local configurations, check GPU topologies, run autobatching memory limits checks, initialize MLflow tracking, and save/upload weights to MinIO/S3.
    *   `trainer/gpu_utils.py`: Monitors GPU temperatures, calculates capability parameters, and checks PyTorch CUDA integrations.

### 5. `wFabricSecurity` (Fabric zero Trust System)
*   **Module structure**:
    *   `wFabricSecurity.py`: Houses the central middleware coordinating rate-limiting (`TokenBucket` algorithm), exponential retry handlers, SHA-256 hash checks on local source code files to verify integrity, and digital signatures validation via ECDSA P-256 public keys.

### 6. `ProcessAudio` (Audio Data Augmentation & Extraction)
*   **Module structure**:
    *   `AudioAugmentation.py`: Formulates pitch shift, speed stretches, and background noise additions.
    *   `Features.py`: Declares `Features` inheriting from Scikit-Learn transformers. Computes MFCC, ZCR, Spectral Rolloff, Spectral Centroid, RMS, and Mel-spectrograms.

---

## 🛠️ 4. Shared Technical Implementations

Across William's Python libraries, several architectural patterns are consistently repeated:

1.  **Pydantic v2 Mappings**: Models are declared using Pydantic fields. Database classes serialize Python dictionaries using `model_dump(mode='json')` and deserialize SQL rows using type validation hooks.
2.  **SQLite WAL optimization**: SQLite databases consistently execute the following initialization commands:
    ```sql
    PRAGMA journal_mode=WAL;
    PRAGMA synchronous=OFF;
    PRAGMA cache_size=-10000;
    PRAGMA busy_timeout=60000;
    ```
3.  **Automatic Documentation (`examples_readme.py`)**: A utility python script found inside package folders. It automatically traverses directories, reads module comments, extracts code snippets, and builds a comprehensive API guide in the local `README.md`.
