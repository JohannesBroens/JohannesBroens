# Johannes Brøns Christensen

Machine learning engineer with a mathematical and statistical foundation, working across deep learning, time-series forecasting, high-performance computing, and scientific data analysis. B.Sc. in Machine Learning & Data Science from the University of Copenhagen (DIKU), with coursework in measure theory, probabilistic inference, and numerical optimization. I build systems that bridge theoretical rigour and production-grade engineering — from CUDA-accelerated neural networks in C to walk-forward backtesting pipelines for European electricity markets.

---

## Education

### B.Sc. in Machine Learning & Data Science — University of Copenhagen (DIKU), 2019–2023

| | |
|---|---|
| **Mathematics & Statistics** | Probability Theory & Statistics, Linear Algebra, Lebesgue Integral & Measure Theory, Models for Complex Systems |
| **Machine Learning & AI** | Advanced Deep Learning, Medical Image Analysis, Probabilistic Graphical Models |
| **Computer Science** | Algorithms & Data Structures, High-Performance Programming (C, CUDA, OpenMP) |
| **Applied Research** | Satellite Image Segmentation (collab. with NASA & IGN), BSc Thesis with DMI |

---

## Professional Experience

### Novo Nordisk — Data & Analytics Specialist / Associate IT Operations Manager

**January 2024 – January 2026**

* Built Python analytics tooling for operational insights across IT/OT environments in a regulated pharmaceutical setting.
* Engineered SQL data models and automated ETL workflows for large-scale industrial reporting.
* Applied statistical analysis on incident and root-cause trends to improve infrastructure reliability.
* Deployed monitoring solutions (SCOM, SquaredUp, Grafana) for real-time critical infrastructure observability.
* Developed an LSTM-based recurrent neural network for predictive maintenance, integrated with OPC-UA data streams.

---

## Selected Projects

### European Electricity Price Forecasting — [`eu-electricity-forecasting`](https://github.com/JohannesBroens/eu-electricity-forecasting)

XGBoost-based day-ahead price forecasting pipeline for 21 European bidding zones with walk-forward backtesting and trading strategy evaluation.

* Dual forecasting modes: single-model and per-hour XGBoost with lag features respecting market gate closures.
* Feature engineering from heterogeneous sources: Energinet, ENTSO-E Transparency Platform, and Open-Meteo weather data (temperature, wind speed, solar irradiance).
* Walk-forward backtesting engine with transaction cost modelling across multiple bidding zones.
* 108 unit tests, data completeness gates, imputation monitoring, and model drift detection.

### Multi-Language ML Benchmark — [`ml-language-playground`](https://github.com/JohannesBroens/ml-language-playground)

Systematic benchmarking of MLP and CNN (LeNet-5) implementations across C, Rust, and Python — 18 variants spanning CPU and GPU backends.

* Custom CUDA kernels, cuBLAS FFI bindings (Rust), cuDNN integration, and OpenMP parallelisation.
* Peak GPU throughput: 8.92M samples/s (C CUDA), 8.21M samples/s (Rust cuBLAS); 5–15x GPU advantage over CPU at scale.
* Mathematical documentation of forward/backward propagation, im2col convolution, and pooling operations.
* Automated benchmarking pipeline with reproducible caching and successive-halving hyperparameter tuning.

### Satellite Image Segmentation for Arctic Mapping — [`Automatic-Satelitte-Island-Discovery`](https://github.com/JohannesBroens/Automatic-Satelitte-Island-Discovery)

Collaborative research with NASA, IGN, and DIKU on segmentation of Greenland's coastline from satellite imagery.

* U-Net architecture (PyTorch, segmentation_models_pytorch) achieving 0.87 IoU on high-resolution ortho-rectified .tif imagery.
* Geospatial preprocessing with Rasterio and GeoPandas; shapefile-based mask generation.
* Trained on NVIDIA RTX A6000 (CUDA 11.8); optimised inference for large-scale geospatial datasets.

### Automated Quality Control of Climate Data (BSc Thesis) — [`Climate-Data-QC`](https://github.com/JohannesBroens/Machine-Learning-based-Automatic-Quality-Control-of-Greenlantic-Climate-Data)

Bachelor's thesis in collaboration with the Danish Meteorological Institute (DMI).

* Designed and benchmarked Random Forest, XGBoost, Logistic Regression, and MLP architectures for faulty sensor detection.
* Analysed DMI's ETL pipelines and manual validation workflows to identify automation opportunities.
* Reduced manual overhead for climatologists through automated anomaly detection on Greenlandic weather station data.

### Uncertainty Estimation in Meteorological Measurements — [`MetaMeter`](https://github.com/JohannesBroens/MetaMeter)

Extension of the climate data QC work toward formal uncertainty quantification in global meteorological observations. Combines statistical methods with ML for quality control and data homogenisation.

### Hidden Markov Model for Visual Attention Analysis

Probabilistic graphical model for simulating and analysing visual attention patterns from neural spike data.

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
| **ML / DL** | PyTorch, PyTorch Lightning, TensorFlow, Scikit-Learn, XGBoost, MLflow |
| **Methods** | Deep learning (CNNs, LSTMs, U-Net), probabilistic graphical models (HMMs, EM), ensemble methods, time-series forecasting, anomaly detection, uncertainty quantification |
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
