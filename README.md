<p align="center">
  <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a>
  <a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Data-Versioning-Platform/stargazers"><img src="https://img.shields.io/github/stars/ishandutta2007/Awesome-Data-Versioning-Platform?style=flat-square&logo=github" alt="GitHub_Stars"/></a>
  <a href="https://github.com/ishandutta2007/Awesome-Data-Versioning-Platform/network/members"><img src="https://img.shields.io/github/forks/ishandutta2007/Awesome-Data-Versioning-Platform?style=flat-square&logo=github" alt="GitHub Forks"/></a>
  <a href="https://github.com/ishandutta2007/Awesome-Data-Versioning-Platform/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-green.svg?style=flat-square" alt="License"/></a>
  <a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>
</p>

<p align="center">
  <img src="assets/banner.svg" alt="Awesome Data Versioning Platform Banner" width="100%" />
</p>

# 🚀 Awesome Data Versioning Platform Ecosystem

> **A curated, comprehensive guide to top SaaS platforms & open-source projects for Data Versioning, Git-for-Data, Data Lake Branching, Model Registries & Reproducible MLOps.**

---

## 📌 Executive Overview & Market Context

Data versioning allows data scientists, ML engineers, and enterprise platform teams to version datasets, database tables, and machine learning models with standard software git semantics—enabling zero-copy branching, time-travel queries, atomic commits, and auditability.

* **Open-Source Standardization & Consolidation**: The data versioning landscape has entered a production-proven era. Notably, **lakeFS** (Treeverse) acquired the **DVC** team in November 2025, bringing object-storage data lake branching and file-based ML pipeline tracking under one roof. Tools like **Dolt** (row-level database Git), **Nessie** (Iceberg catalog branching), and **MLflow** (model registry & tracking) form the foundation of modern reproducible AI pipelines.

---

## 📑 Table of Contents

- [☁️ SaaS / Hosted Data Versioning Platforms](#-saas--hosted-data-versioning-platforms)
- [🔓 Open-Source Data Versioning Projects](#-open-source-data-versioning-projects)
- [🤝 How to Contribute](#-how-to-contribute)
- [💖 Support & Community](#-support--community)
- [📈 Star History](#-star-history)
- [📜 Disclaimer](#-disclaimer)

---

## ☁️ SaaS / Hosted Data Versioning Platforms

📊 **Market Intelligence & Dynamics**: The global Data Versioning and MLOps sector is estimated at **~$4.2 Billion in 2026** (projected to reach **$16.5 Billion by 2030** at a ~31% CAGR). The market is currently **moderately fragmented**, with active strategic consolidation (e.g., lakeFS acquiring DVC, HPE acquiring Pachyderm) standardizing data lake control planes and model lifecycle tracking.

The table below summarizes leading managed SaaS solutions, sorted by **Company Scale & Valuation (Descending)**:

| 🏢 Platform / SaaS Product | 📈 Scale & Valuation | 💰 Starting Tier Price | 🎁 Free Tier / Trial Limit |
| :--- | :--- | :--- | :--- |
| **[Pachyderm (HPE MLDM)](https://www.pachyderm.com/)** <br> Data versioning and automated pipeline orchestration engine for Kubernetes. | **$28.5 Billion Revenue** <br>*(Parent HPE; acquired 2023)* | **$1,000 / month** <br>*(Contact HPE Sales for Enterprise)* | **14-day Enterprise Free Trial** <br>*(Self-hosted Community Edition is free)* |
| **[Weights & Biases Artifacts](https://wandb.ai/)** <br> Enterprise ML artifact, dataset, and model lineage tracking within W&B platform. | **$1.25 Billion Valuation** <br>*(~$50M+ ARR)* | **$60 / user / month** <br>*(Pro Plan)* | **5 GB Storage & 1 GB Ingestion/mo** <br>*(Up to 5 team seats)* |
| **[lakeFS Cloud](https://lakefs.io/)** <br> Managed zero-copy data lake branching, time-travel, and S3-compatible data version control. | **$51 Million Funding** <br>*(Acquired DVC team Nov 2025)* | **$0.007 / GB / month** <br>*(Cloud Standard starts $250/mo)* | **15-day Enterprise Cloud Free Trial** <br>*(Full feature access)* |
| **[Iterative Studio](https://iterative.ai/)** <br> Cloud experiment tracking and model management platform for DVC & Git. | **$25 Million Funding** <br>*(Aligned with lakeFS ecosystem)* | **$50 / user / month** <br>*(Team Plan)* | **5 Team Members & 5 Active Experiments** <br>*(Free forever)* |
| **[DoltHub](https://www.dolthub.com/)** <br> Hosted cloud platform for version-controlled, MySQL-compatible SQL databases. | **$21 Million Funding** <br>*(~$1.5M ARR)* | **$5 / month** <br>*(Pro Plan for private DBs)* | **100 MB Private Storage Free** <br>*(Unlimited public databases)* |
| **[ClearML Pro](https://clear.ml/)** <br> Unified MLOps platform featuring data management, artifact versioning, and tracking. | **$16 Million Funding** <br>*(~$4.7M ARR)* | **$15 / user / month** <br>*(Pro Plan + cloud usage)* | **3 Team Users, 100 GB Storage & 1M API Calls/mo** |
| **[DagsHub](https://dagshub.com/)** <br> Integrated platform connecting Git, DVC, and MLflow for unified dataset/model versioning. | **$3.6 Million Funding** <br>*(~$1.5M ARR)* | **$99 / user / month** <br>*(Team Plan billed annually)* | **20 GB DagsHub Storage & 100 Private Experiments** <br>*(Unlimited public repos)* |

---

## 🔓 Open-Source Data Versioning Projects

Production-proven open-source repositories powering data lakes, relational databases, feature stores, and ML artifacts. 

Sorted by **GitHub Stars_Count (Descending)**:

| 📦 Repository & Project Name | ⭐ GitHub_Stars & Link | 📝 Primary Description & Key Use Cases |
| :--- | :---: | :--- |
| **[MLflow](https://github.com/mlflow/mlflow)** <br> *(mlflow/mlflow)* | [<img src="https://img.shields.io/github/stars/mlflow/mlflow?style=social&color=white" alt="MLflow Stars"/>](https://github.com/mlflow/mlflow/stargazers) | **Open-source MLOps platform**. Provides Model Registry, dataset versioning, experiment tracking, and artifact logging. |
| **[Dolt](https://github.com/dolthub/dolt)** <br> *(dolthub/dolt)* | [<img src="https://img.shields.io/github/stars/dolthub/dolt?style=social&color=white" alt="Dolt Stars"/>](https://github.com/dolthub/dolt/stargazers) | **Git for Data**. MySQL-compatible relational database with native row-level Git semantics (commit, branch, merge, diff). |
| **[DVC (Data Version Control)](https://github.com/iterative/dvc)** <br> *(iterative/dvc)* | [<img src="https://img.shields.io/github/stars/iterative/dvc?style=social&color=white" alt="DVC Stars"/>](https://github.com/iterative/dvc/stargazers) | **Git-like version control for ML datasets & models**. Manages pointer files in Git with remote cache storage (S3/GCS/Azure). |
| **[Git LFS](https://github.com/git-lfs/git-lfs)** <br> *(git-lfs/git-lfs)* | [<img src="https://img.shields.io/github/stars/git-lfs/git-lfs?style=social&color=white" alt="Git LFS Stars"/>](https://github.com/git-lfs/git-lfs/stargazers) | **Git Large File Storage**. Replaces large binary files (datasets, model weights) with text pointers inside Git repositories. |
| **[Great Expectations](https://github.com/great-expectations/great_expectations)** <br> *(great-expectations/great_expectations)* | [<img src="https://img.shields.io/github/stars/great-expectations/great_expectations?style=social&color=white" alt="Great Expectations Stars"/>](https://github.com/great-expectations/great_expectations/stargazers) | **Data quality & validation framework**. Validates, documents, and profiles datasets across pipeline versions. |
| **[Kedro](https://github.com/kedro-org/kedro)** <br> *(kedro-org/kedro)* | [<img src="https://img.shields.io/github/stars/kedro-org/kedro?style=social&color=white" alt="Kedro Stars"/>](https://github.com/kedro-org/kedro/stargazers) | **Data science framework**. Creates reproducible, maintainable data pipelines with integrated dataset versioning capabilities. |
| **[Apache Iceberg](https://github.com/apache/iceberg)** <br> *(apache/iceberg)* | [<img src="https://img.shields.io/github/stars/apache/iceberg?style=social&color=white" alt="Apache Iceberg Stars"/>](https://github.com/apache/iceberg/stargazers) | **High-performance open table format for huge analytic datasets**. Enables snapshot isolation and table time-travel. |
| **[Delta Lake](https://github.com/delta-io/delta)** <br> *(delta-io/delta)* | [<img src="https://img.shields.io/github/stars/delta-io/delta?style=social&color=white" alt="Delta Lake Stars"/>](https://github.com/delta-io/delta/stargazers) | **Open-source storage layer**. Brings ACID transactions, data versioning (time travel), and schema enforcement to data lakes. |
| **[Flyte](https://github.com/flyteorg/flyte)** <br> *(flyteorg/flyte)* | [<img src="https://img.shields.io/github/stars/flyteorg/flyte?style=social&color=white" alt="Flyte Stars"/>](https://github.com/flyteorg/flyte/stargazers) | **Production-grade data & ML orchestration engine**. Tracks execution provenance, dataset lineage, and typed artifacts. |
| **[Feast](https://github.com/feast-dev/feast)** <br> *(feast-dev/feast)* | [<img src="https://img.shields.io/github/stars/feast-dev/feast?style=social&color=white" alt="Feast Stars"/>](https://github.com/feast-dev/feast/stargazers) | **Open-source feature store for ML**. Manages, serves, and versions point-in-time correct features for model training & inference. |
| **[Pachyderm (Community)](https://github.com/pachyderm/pachyderm)** <br> *(pachyderm/pachyderm)* | [<img src="https://img.shields.io/github/stars/pachyderm/pachyderm?style=social&color=white" alt="Pachyderm Stars"/>](https://github.com/pachyderm/pachyderm/stargazers) | **Data versioning & data-driven pipelines on Kubernetes**. Offers Git-like data version control with automated lineage tracking. |
| **[lakeFS](https://github.com/treeverse/lakeFS)** <br> *(treeverse/lakeFS)* | [<img src="https://img.shields.io/github/stars/treeverse/lakeFS?style=social&color=white" alt="lakeFS Stars"/>](https://github.com/treeverse/lakeFS/stargazers) | **Git-for-data platform for data lakes**. Zero-copy branching, time travel, and atomic commits on S3, GCS, and Azure Blob storage. |
| **[CML (Continuous Machine Learning)](https://github.com/iterative/cml)** <br> *(iterative/cml)* | [<img src="https://img.shields.io/github/stars/iterative/cml?style=social&color=white" alt="CML Stars"/>](https://github.com/iterative/cml/stargazers) | **Open-source library for CI/CD in ML projects**. Auto-generates metrics & dataset diff reports directly in GitHub/GitLab PRs. |
| **[ModelDB](https://github.com/VertaAI/modeldb)** <br> *(VertaAI/modeldb)* | [<img src="https://img.shields.io/github/stars/VertaAI/modeldb?style=social&color=white" alt="ModelDB Stars"/>](https://github.com/VertaAI/modeldb/stargazers) | **Model versioning and metadata management system**. Tracks machine learning models, pipelines, and execution metadata. |
| **[Nessie](https://github.com/projectnessie/nessie)** <br> *(projectnessie/nessie)* | [<img src="https://img.shields.io/github/stars/projectnessie/nessie?style=social&color=white" alt="Nessie Stars"/>](https://github.com/projectnessie/nessie/stargazers) | **Transactional catalog for data lakes**. Provides Git-like multi-table branching, tagging, and atomic commits for Apache Iceberg. |
| **[Quilt](https://github.com/quiltdata/quilt)** <br> *(quiltdata/quilt)* | [<img src="https://img.shields.io/github/stars/quiltdata/quilt?style=social&color=white" alt="Quilt Stars"/>](https://github.com/quiltdata/quilt/stargazers) | **Data package manager & versioning tool**. Manages AWS S3 data packages with version control, docs, and visualization. |
| **[ChiveSave](https://github.com/CHIVE-AI/chivesave-community-backend)** <br> *(CHIVE-AI/chivesave-community-backend)* | [<img src="https://img.shields.io/github/stars/CHIVE-AI/chivesave-community-backend?style=social&color=white" alt="ChiveSave Stars"/>](https://github.com/CHIVE-AI/chivesave-community-backend/stargazers) | **Self-hosted AI artifact versioning backend**. Built with FastAPI & PostgreSQL for private artifact storage and metadata restore. |

---

## 🤝 How to Contribute

Contributions are warmly welcomed! Please follow these simple guidelines:

1. **Fork** the repository.
2. Add your suggested project/tool to `README.md` maintaining alphabetical or specified sorting order.
3. Ensure description includes key features, starting price/tier (for SaaS), or GitHub repository stargazers link (for Open Source).
4. Submit a **Pull Request** with a descriptive summary of changes.

Check out our awesome ecosystem list collection at [Awesome-Awesome-Awesome](https://github.com/ishandutta2007/Awesome-Awesome-Awesome)!

---

## 💖 Support & Community

If you find this repository helpful, please consider showing your support:

- 🌟 **Star this repository** to help others discover data versioning tools!
- 🔀 **Fork & Share** with your team, ML engineers, and data community.
- 💬 **Join our Discord**: Connect with fellow data professionals on [Discord](https://discord.gg/jc4xtF58Ve).
- ☕ **Sponsor & Buy a Coffee**: Support ongoing open-source curation on [GitHub Sponsors](https://github.com/sponsors/ishandutta2007).

---

## 📈 Star History

[![Star History Chart](https://star-history.dera.page/svg?repos=ishandutta2007/Awesome-Data-Versioning-Platform&type=date&legend=top-left)](https://star-history.dera.page/#ishandutta2007/Awesome-Data-Versioning-Platform&type=date&legend=top-left)

---

## 📜 Disclaimer

This list is community-curated for informational and educational purposes. Product details, pricing, and company metrics are accurate based on public data sources as of late 2026. Data versioning software handles critical business data and AI model assets—ensure proper security controls and data governance compliance before enterprise deployment.
