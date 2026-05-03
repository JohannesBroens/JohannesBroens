# Johannes Brøns Christensen

> **Now (May 2026):** Junior Data & ML Engineer at **Epiq Energy ApS**, Copenhagen — applied ML in the European energy domain.

Machine learning engineer with a mathematical and statistical foundation, working across deep learning, time-series forecasting, high-performance computing, and scientific data analysis. B.Sc. in Machine Learning & Data Science from the University of Copenhagen (DIKU), with coursework in measure theory, probability theory, and high-performance programming. I build systems that bridge theoretical rigour and production-grade engineering — from CUDA-accelerated neural networks in C to walk-forward backtesting pipelines for European electricity markets.

---

## Education

### B.Sc. in Machine Learning & Data Science — University of Copenhagen (DIKU), 2019–2023

| | |
|---|---|
| **Mathematics & Statistics** | Probability Theory & Statistics, Linear Algebra, Lebesgue Integral & Measure Theory, Models for Complex Systems |
| **Machine Learning & AI** | Introduction to Machine Learning, Advanced Deep Learning, Medical Image Analysis |
| **Computer Science** | Algorithms & Data Structures, High-Performance Programming (C, CUDA, OpenMP) |
| **Applied Research** | Satellite Image Segmentation (collab. with IGN), BSc Thesis with DMI |

---

## Professional Experience

### Epiq Energy ApS — Junior Data & ML Engineer

**May 2026 – present**

Applied ML in the European energy domain.

### Novo Nordisk — Associate IT Operation Manager

**January 2024 – January 2026**

* Managed local IT infrastructure, automation (OT) systems, and MES support in a GMP-regulated pharmaceutical manufacturing environment.
* Performed statistical analysis on incident and root-cause trends to support reliability improvements.
* Deployed monitoring solutions (SCOM, SquaredUp, Grafana) for real-time IT/OT infrastructure observability.
* Self-initiated cross-team data & analytics work: built Python tooling and SQL data models for operational insights.
* Self-initiated: developed an LSTM-based recurrent neural network for predictive maintenance, integrated with OPC-UA data streams.

---

## Selected Projects

### European Electricity Price Forecasting — [`eu-electricity-forecasting`](https://github.com/JohannesBroens/eu-electricity-forecasting)

XGBoost-based day-ahead price forecasting pipeline for 21 European bidding zones with walk-forward backtesting and trading strategy evaluation.

* Dual forecasting modes: single-model and per-hour XGBoost with lag features respecting market gate closures.
* Feature engineering from heterogeneous sources: Energinet, ENTSO-E Transparency Platform, and Open-Meteo weather data (temperature, wind speed, solar irradiance).
* Walk-forward backtesting engine with transaction cost modelling across multiple bidding zones.
* 108 unit tests, data completeness gates, imputation audit logging, and model drift detection.

### Multi-Language ML Benchmark — [`ml-language-playground`](https://github.com/JohannesBroens/ml-language-playground)

Systematic benchmarking of neural networks (MLP, CNN/LeNet-5) and a broader algorithm catalogue (regression, tree ensembles, sequence models, Gaussian Process, HMM, unsupervised) across C, Rust, and Python — CPU and GPU backends.

* Custom CUDA kernels, cuBLAS FFI bindings (Rust), cuDNN integration, and OpenMP parallelisation.
* Peak GPU throughput: 8.92M samples/s (C CUDA), 8.21M samples/s (Rust cuBLAS); 5–15× GPU advantage over CPU at scale.
* Mathematical documentation of forward/backward propagation, im2col convolution, and pooling operations.
* Automated benchmarking pipeline with reproducible caching and successive-halving hyperparameter tuning.

### Satellite Image Segmentation for Arctic Mapping — [`Automatic-Satelitte-Island-Discovery`](https://github.com/JohannesBroens/Automatic-Satelitte-Island-Discovery)

Project outside course scope at DIKU, in collaboration with the Department of Geosciences and Natural Resource Management (IGN) at the University of Copenhagen — semantic segmentation of land regions along Greenland's coastline.

* U-Net architecture (PyTorch, segmentation_models_pytorch) on high-resolution 4-band PlanetScope imagery; test-set accuracy 0.92, IoU 0.53.
* Geospatial preprocessing with Rasterio and GeoPandas; shapefile-based mask generation from IGN-provided ground truth.
* Trained on an NVIDIA RTX A6000 GPU cluster (CUDA 11.8); optimised inference for large-scale geospatial datasets.

### Automated Quality Control of Climate Data (BSc Thesis) — [`Climate-Data-QC`](https://github.com/JohannesBroens/Machine-Learning-based-Automatic-Quality-Control-of-Greenlantic-Climate-Data)

Bachelor's thesis in collaboration with the Danish Meteorological Institute (DMI).

* Designed and benchmarked three structurally distinct ML architectures for faulty sensor detection.
* Analysed DMI's ETL pipelines and manual validation workflows to identify automation opportunities.
* Reduced manual overhead for climatologists through automated anomaly detection on Greenlandic weather station data.

### Hidden Markov Model for Visual Attention Analysis

Probabilistic graphical model for simulating and analysing visual attention patterns from neural spike data (course project: *Models for Complex Systems*).

* Forward simulation, exact inference (variable elimination, message passing), and approximate inference (logistic regression).
* Hard-assignment EM algorithm for parameter learning; validated on simulated and real-world neural datasets.

### Native X11 MCP Server — [`x11-mcp`](https://github.com/JohannesBroens/x11-mcp)

Bare-metal Linux desktop automation server for Claude Code, using python-xlib, python-uinput, and AT-SPI.

* Framebuffer capture, kernel-level input simulation, and accessibility-tree integration.
* Extended with voice control pipeline ([`x11-mcp-voice`](https://github.com/JohannesBroens/x11-mcp-voice)): openwakeword → NVIDIA Parakeet STT → Claude → piper-tts.

---

## Technical Skills

| | |
|---|---|
| **Languages** | Python, C, SQL, R |
| **ML / DL** | PyTorch, PyTorch Lightning, TensorFlow, Scikit-Learn, XGBoost, OpenCV |
| **Methods** | Deep learning (CNNs, LSTMs, U-Net), probabilistic graphical models (HMMs, EM), ensemble methods, time-series forecasting, anomaly detection |
| **HPC / Systems** | CUDA, cuBLAS, cuDNN, OpenMP |
| **Data Engineering** | ETL pipelines, Pandas, NumPy, Rasterio, GeoPandas, Alteryx |
| **Visualisation** | Matplotlib, Plotly |
| **Infrastructure** | Linux/UNIX, Git, Docker, MLOps |

---

## Academic Service & Teaching

* **Teaching Assistant** — Empirical Methodologies & Theory of Science (2021–2023). Research methodology and academic reasoning.
* **Teaching Assistant** — Introduction to Programming (2021). Python fundamentals for first-year students.
* **Student Mediator** — ML & Data Science programme representative at DIKU. Curriculum feedback and student outreach.

---

## Contact

* **Email:** j.brons.christensen@gmail.com
* **LinkedIn:** [linkedin.com/in/johannes-broens-christensen](https://linkedin.com/in/johannes-broens-christensen/)
