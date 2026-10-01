# Awesome-Data-Versioning-Platform

# Top Data Versioning Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Dataset Versioning, Model Artifact Management, Git-for-Data & Reproducibility*
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Data Versioning**. These tools help data scientists, ML engineers, and data platform teams version datasets, models, and artifacts the same way developers version code—with commits, branches, tags, and full audit history.

**Examples** include DVC Studio, lakeFS, Pachyderm, DoltHub, Weights & Biases Artifacts, ClearML, DagsHub, Project Nessie, Iterative Studio, and Git-LFS (the category leaders).

**Open-source emphasis**: Data versioning has a **mature and production-proven open-source ecosystem**. **lakeFS** and **DVC** are now under one roof—lakeFS acquired the DVC team in November 2025 . **Dolt** brings full Git semantics into the database itself with 19,391 stars . **Nessie** provides Git-like branching for Iceberg data lakes . **DagsHub** connects Git, DVC, and MLflow for a unified MLOps platform . This section documents these production-grade solutions.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[lakeFS Cloud](https://lakefs.io/)**
  Managed version of lakeFS, the leading Git-for-data platform for data lakes. Provides zero-copy branching, time travel, and atomic commits on object storage. **Acquired the DVC team in November 2025**, unifying the data versioning standard.

- **[DVC Studio](https://studio.iterative.ai/)**
  Cloud hub for DVC-based experiment tracking and model management. Centralizes projects, experiments, and models with Git-based versioning. **Now part of the lakeFS ecosystem** following the November 2025 acquisition.

- **[Weights & Biases Artifacts](https://wandb.ai/)**
  ML artifact versioning within the W&B platform. Tracks datasets, models, and dependencies with lineage, aliases, and tags .

- **[Iterative Studio](https://iterative.ai/)**
  DVC's commercial offering for experiment tracking and model management. Now aligned with lakeFS direction.

- **[DagsHub](https://dagshub.com/)**
  Platform connecting Git, DVC, and MLflow for a unified MLOps experience. Hosts datasets and models with versioning and lineage . Free tier includes unlimited public repos and up to 100 tracked experiments in private repos; Team at $99/user/month .

- **[ClearML](https://clear.ml/)**
  MLOps platform with artifact and dataset versioning. Provides experiment tracking, data management, and model registry.

- **[Pachyderm](https://www.pachyderm.com/)**
  Data versioning and pipeline platform for Kubernetes. Provides Git-like versioning for data with automatic pipeline triggering on changes.

- **[DoltHub](https://www.dolthub.com/)**
  Cloud platform for Dolt databases. Provides hosted version-controlled SQL databases with collaboration features.

## Open-Source GitHub Projects

### Data Lake & Catalog Versioning

- **[lakeFS](https://github.com/treeverse/lakeFS)**
  **The leading Git-for-data platform for data lakes.** **4,054 stars, 328 forks**. Provides **zero-copy branching** (instant, no data duplication), **atomic commits**, **time travel** to historical versions, and **S3 API compatibility** . Works with **S3, Azure Blob, GCS** and integrates with **Iceberg/Delta Lake**. Scale: petabytes. Format: any (object storage). **Go-based**. **Acquired DVC team November 2025**—now the unified standard for data versioning.

- **[Nessie](https://github.com/projectnessie/nessie)**
  **Transactional catalog for data lakes with Git-like semantics.** **1,044+ stars**. Provides **branch, tag, merge, and multi-table commits** for Apache Iceberg tables. **Only product in the lakehouse catalog space that versions the entire catalog** with branches, tags, merges, and cross-table atomic commits. Works with **Spark, Trino, Flink, Dremio** and other Iceberg-compatible engines. **Apache-2.0**.

- **[EpochFS](https://github.com/epochfs/epochfs)**
  **Versioned cloud file system with Git-like branching and exabyte scale.** **Apache-2.0 licensed**. Provides zero-copy branching, atomic commits, and time travel on object storage.

### ML Dataset & Artifact Versioning

- **[DVC (Data Version Control)](https://github.com/iterative/dvc)**
  **Git-like version control for ML datasets and models.** **13,212 stars, 1,148 forks**. Stores **pointer files in Git** while keeping actual data in remote cache (S3, GCS, Azure, etc.). **Key features**: `dvc add` for dataset tracking; `dvc repro` for reproducible pipelines (DAG); `dvc exp run` for experiment management; `dvc diff` for change detection. Granularity: file-level (can't show row-level changes). **Best for**: Small ML projects and reproducible pipelines. **Python-based**. **Note**: DVC team acquired by lakeFS (November 2025); lakeFS recommended for new projects.

- **[ChiveSave](https://github.com/CHIVE-AI/chivesave-community-backend)**
  **Self-hosted, community-driven AI artifact versioning backend.** **FastAPI + PostgreSQL**. **Core features**: **Version Saving** (securely upload and store new versions of AI artifacts with descriptive names, detailed descriptions, and custom JSON metadata); **Preview** (retrieve comprehensive metadata for any version without downloading); **Restore** (activate any previous version by copying to "current active" directory); **Version Database** (PostgreSQL backend for reliable metadata storage). **Authentication**: JWT-based with user registration and role-based access control. **Deployment**: Docker Compose for easy setup. **Perfect for**: Individual researchers, small teams, or community-driven AI initiatives.

- **[ModelDB](https://github.com/VertaAI/modeldb)**
  **Open-source model versioning and metadata management system.** **1,668 stars, 375 forks**. Designed to track ML models, versions, and associated metadata throughout their lifecycle.

### In-Database Version Control

- **[Dolt](https://github.com/dolthub/dolt)**
  **Git for Data—version control built into the database kernel.** **19,391 stars, 593 forks**. MySQL-compatible SQL database with **native Git semantics** (commit, branch, merge, diff, clone, push/pull) operating at **row-level granularity**. **Key difference from file-based tools**: Version control is inside the database, understanding every row and storing changes as immutable increments. **Best for**: Applications requiring row-level data versioning, audit trails, or collaborative data editing.

### Additional Strong Open-Source Options

- **Data Lake Versioning**: **lakeFS** (zero-copy branching, petabyte scale, S3-compatible), **Nessie** (Iceberg catalog with Git semantics, multi-table commits), **EpochFS** (versioned cloud file system, exabyte scale) .
- **ML Dataset Versioning**: **DVC** (Git-like, file-level, 13k+ stars), **ChiveSave** (self-hosted AI artifact backend, FastAPI + PostgreSQL), **ModelDB** (model versioning and metadata, 1,668 stars) .
- **In-Database**: **Dolt** (row-level Git for data, MySQL-compatible, 19k+ stars) .
- **Metadata**: **MLflow** (Model Registry for versioning and lifecycle management, Apache-2.0) .

**Frameworks for building custom systems**: Combine **lakeFS** for data lake versioning with zero-copy branching, **DVC** for ML dataset and pipeline versioning, **Nessie** for Iceberg catalog branching and multi-table commits, **Dolt** for row-level in-database versioning, and **ChiveSave** for self-hosted AI artifact management. Add **PostgreSQL** for metadata persistence and **Docker** for deployment.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Data versioning platforms handle sensitive datasets and models; ensure proper access controls and compliance with data governance policies.
- **Open-source reality**: The open-source ecosystem for data versioning is **mature and production-proven**. **lakeFS** and **DVC** are now under one roof following the November 2025 acquisition, with lakeFS recommended for production data lakes and DVC still viable for small ML projects . **Nessie** remains the only catalog providing Git-like branching across Iceberg tables . **Dolt** brings row-level Git semantics into the database kernel with 19,391 stars . **ChiveSave** provides a self-hosted AI artifact backend for teams wanting full control . The open-source path is **genuinely viable** for organizations seeking data versioning without vendor lock-in.

---

**Made for data engineers, ML engineers, MLOps practitioners, and data platform teams.**
Let's make data versioning more open, transparent, and reproducible.
