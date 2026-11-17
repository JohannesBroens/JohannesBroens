# Johannes Brøns Christensen

> **Now:** Junior Data & ML Engineer at **Epiq Energy ApS**, Copenhagen (since May 2026) — Azure-based data ingestion and models for intraday electricity trading on Nord Pool.

Data & ML engineer with a mathematical and statistical foundation. B.Sc. in Machine Learning & Data Science from the University of Copenhagen (DIKU), with coursework in measure theory, probability theory, and high-performance programming. I like problems where you have to decide which of a very large number of measurements you can trust — from meteorological sensor data in my bachelor thesis with DMI to electricity-market data today — and side projects that go close to the hardware, from CUDA neural networks in C to Linux desktop automation for AI agents.

---

## Education

### B.Sc. in Machine Learning & Data Science — University of Copenhagen (DIKU), 2019–2023

| | |
|---|---|
| **Mathematics & Statistics** | Probability Theory & Statistics, Linear Algebra, Lebesgue Integral & Measure Theory, Models for Complex Systems |
| **Machine Learning & AI** | Introduction to Machine Learning, Advanced Deep Learning, Medical Image Analysis |
| **Computer Science** | Algorithms & Data Structures, High Performance Programming & Systems |
| **Applied Research** | Satellite image segmentation (project outside course scope, with IGN), BSc thesis with DMI (grade 12) |

---

## Professional Experience

### Epiq Energy ApS — Junior Data & ML Engineer

**May 2026 – present** · Copenhagen

* Azure-based ingestion layer consolidating market data and a wide range of external sources into one shared dataset, with incremental, idempotent loading (re-runs and backfills without duplicates).
* Models and estimates for intraday trading (SIDC) on Nord Pool, and backtests validated against trades that actually executed.
* Pipeline and model monitoring in Grafana.

### Novo Nordisk A/S — Associate IT Operation Manager

**January 2024 – January 2026** · Kalundborg

IT operations and infrastructure support for GMP pharmaceutical manufacturing, with a data & analytics focus.

* 1st/2nd-line support, 24/7 on-call duty, Windows/Linux infrastructure operations, and PAS-X / LMES+ MES support.
* Designed ServiceNow dashboards, reports and KPIs for incident and problem trends; built Power BI dashboards and SQL data models.
* Set up SCOM, SquaredUp and Grafana monitoring for IT/OT infrastructure.
* Prepared the document corpus (~400 documents, 256 knowledge-base articles, ~4.3k incidents) and prompt context for an internal GPT-4 support chatbot.
* Explored (self-initiated) ML approaches for anomaly detection and predictive maintenance.

---

## Selected Projects

### European Electricity Price Forecasting — [`eu-electricity-forecasting`](https://github.com/JohannesBroens/eu-electricity-forecasting)

XGBoost-based day-ahead price forecasting pipeline for 21 European bidding zones, with walk-forward backtesting.

* Single-model and per-hour XGBoost with lag features that respect market gate closures.
* Data from the ENTSO-E Transparency Platform, Energinet and Open-Meteo weather.
* Data-quality work: DST 23/25-hour handling, rolling z-score outlier detection that keeps genuine negative prices, imputation audit log, schema validation and drift detection.
* 109 tests, GitHub Actions CI and a Dockerfile.

### Multi-Language ML Benchmark — [`ml-language-playground`](https://github.com/JohannesBroens/ml-language-playground)

Benchmarking neural networks (MLP, CNN/LeNet-5) and a broader algorithm catalogue across C, Rust and Python, on CPU and GPU backends.

* 18 backend/device configurations (8 MLP + 10 CNN/LeNet-5): custom CUDA kernels, cuBLAS FFI bindings (Rust), cuDNN and OpenMP.
* Peak MLP throughput 9.7M samples/s (C CUDA, hidden-size sweep, RTX 3070); 9.15M samples/s for Rust cuBLAS in the same sweep.
* Mathematical documentation of forward/backward propagation, im2col convolution and pooling.
* Automated benchmarking pipeline with caching and successive-halving hyperparameter tuning.

### Satellite Image Segmentation of Greenland's Coastline — [`Automatic-Satelitte-Island-Discovery`](https://github.com/JohannesBroens/Automatic-Satelitte-Island-Discovery)

Project outside course scope at DIKU, in collaboration with the Department of Geosciences and Natural Resource Management (IGN), University of Copenhagen.

* U-Net (PyTorch, segmentation_models_pytorch) on 4-band PlanetScope imagery; test-set IoU 0.53 / Dice 0.55 (accuracy 0.92), limited by a very small training set.
* Geospatial preprocessing with Rasterio and GeoPandas; shapefile-based mask generation from IGN ground truth.
* Trained on a Slurm GPU cluster (NVIDIA RTX A6000).

### Automated Quality Control of Climate Data (BSc Thesis) — [`Climate-Data-QC`](https://github.com/JohannesBroens/Machine-Learning-based-Automatic-Quality-Control-of-Greenlantic-Climate-Data)

Bachelor's thesis in collaboration with the Danish Meteorological Institute (DMI), grade 12.

* Designed and compared three classifiers for detecting faulty meteorological sensor readings: logistic regression, XGBoost and a PyTorch MLP, trained on ~41M hourly observations.
* Best model (MLP): balanced accuracy 0.848, AUC 0.822 on a time-ordered test set (XGBoost 0.735 / 0.790, logistic regression 0.650 / 0.718).
* Data extraction from DMI's PostgreSQL database; documented DMI's ETL pipeline and the climatologists' manual validation process.

### Hidden Markov Model for Visual Attention Analysis

Course project in *Models for Complex Systems*: a probabilistic graphical model for simulating and analysing visual-attention patterns from neural spike data — forward simulation, exact inference (variable elimination, message passing), approximate inference (logistic regression) and hard-assignment EM.

### Native X11 MCP Server — [`x11-mcp`](https://github.com/JohannesBroens/x11-mcp)

Bare-metal Linux desktop automation server for Claude Code, using python-xlib, python-uinput and AT-SPI: framebuffer capture, kernel-level input and accessibility-tree integration. 146 tests.

---

## Technical Skills

| | |
|---|---|
| **Languages** | Python, SQL, C, R, Bash, Rust (basic) |
| **ML / DL** | PyTorch, XGBoost, scikit-learn |
| **Methods** | Time-series forecasting, learning-to-rank, image segmentation (U-Net), probabilistic models (HMMs, EM), anomaly detection and data quality on sensor data |
| **HPC** | CUDA, cuBLAS, cuDNN, OpenMP |
| **Data** | ETL and data ingestion, Azure, PostgreSQL, Pandas, NumPy, Rasterio, GeoPandas, Power BI, Alteryx |
| **Tooling** | Linux, Git, Docker, pytest, GitHub Actions, Grafana |

---

## Teaching & Outreach

* **Teaching Assistant** — Empirical Methodologies & Theory of Science, University of Copenhagen (2021–2023): exercise classes and written feedback.
* **Teaching Assistant** — Kickstarting in Programming course, University of Copenhagen (2021).
* **Mediator for Students** — outreach to high-school students for DIKU's Machine Learning & Data Science programme (2021–2023).

---

## Contact

* **Email:** j.brons.christensen@gmail.com
* **LinkedIn:** [linkedin.com/in/johannes-broens-christensen](https://linkedin.com/in/johannes-broens-christensen/)
