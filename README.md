# Yuyao (Phoebe) Wang

![MSc ECE @ University of Alberta](https://img.shields.io/badge/MSc%20ECE-University%20of%20Alberta-informational)
![Focus: Earth Observation ML](https://img.shields.io/badge/Focus-Earth%20Observation%20ML-blue)
![Focus: Scientific Computing](https://img.shields.io/badge/Focus-Scientific%20Computing-blue)
![Python](https://img.shields.io/badge/Code-Python-3776AB?logo=python&logoColor=white)
![C++](https://img.shields.io/badge/Code-C%2B%2B-00599C?logo=c%2B%2B&logoColor=white)
![FPGA / Vitis HLS](https://img.shields.io/badge/Acceleration-FPGA%20%2F%20Vitis%20HLS-6A1B9A)

**Executive summary:**  
I’m an MSc ECE researcher building **machine learning systems for Earth observation** and **high-performance scientific simulation tools**. My work often combines **data engineering, modeling, and systems optimization** to make complex models practical for real-world environments.

**Quick links:**  
[Email](mailto:yuyaow42@gmail.com) • [LinkedIn](https://linkedin.com/in/yuyao-wang) • [GitHub](https://github.com/yuyao-wang)

**Open to:** Machine Learning Engineer • Applied Scientist • Software Engineer (HPC / ML Systems)


## About Me

My interests lie at the intersection of **machine learning**, **geospatial / remote sensing data engineering**, and **systems performance**.

Across my projects, I often encounter a similar challenge: **domain mismatch**. This could appear as cross-sensor differences in satellite imagery, operational constraints in real-world workflows, or hardware limitations when deploying numerical simulations. Much of my work focuses on the engineering required to make models and systems more robust under these shifts.

Current areas I’m exploring include:

- Multi-sensor methane plume detection under domain shifts (remote sensing → domain adaptation)
- Lightweight adaptation techniques for vision backbones (adapters / LoRA-style modules)
- Scientific computing and performance engineering (stiff PDE solvers, CPU–FPGA acceleration)
- Practical workflow systems that reduce operational friction (OCR + role-based auditing)

## Project Showcase

<details>
<summary><b>MethaneSphere — Multi-sensor methane detection (portfolio snapshot)</b></summary>

**Repo:** https://github.com/yuyao-wang/MethaneSphere

**Problem**  
Methane plumes are sparse and transient; single-sensor revisit limitations create a “revisit-time bottleneck”. The goal is to detect plumes more robustly by leveraging multiple satellite domains.

**Approach / Method**  
- Portfolio documents a multi-sensor pipeline concept (Sentinel-2, Landsat 8/9, Sentinel-5P, plus EMIT-based simulation artifacts).  
- Uses a ViT-like “universal backbone + sensor-specific adaptation” framing (sensor-as-domain) with lightweight adapter components.

**Key results / artifacts**  
- Internal comparison snapshot reports improved overall accuracy for “universal + sensor-specific LoRA adapters” vs single-domain baselines (see repo README).  
- Public-safe demo folder includes two toy scripts:
  - EMIT-like hyperspectral → multispectral bandpass simulation
  - Domain-adaptive ViT-style adapter demo (synthetic tensors only)

**Tech stack**  
- Python (public-safe demos use NumPy-style tensors)  
- Full training framework / checkpoints / complete datasets: **unspecified (intentionally withheld pre-publication)**

**How to run / demo**  
- Demo folder: https://github.com/yuyao-wang/MethaneSphere/tree/main/portfolio/demo  
- Run:
  ```bash
  python3 portfolio/demo/emit_bandpass_simulation_demo.py
  python3 portfolio/demo/multidomain_vit_adapter_demo.py
</details>

<details>
<summary><b>MSRE-BC-1D — Real-time multiphysics reactor simulation</b></summary>

**Repo**  
https://github.com/yuyao-wang/MSRE-BC-1D

### Problem

Molten salt reactor dynamics involve **stiff PDE systems** combining:

- neutron diffusion
- delayed neutron kinetics
- thermal hydraulics
- heat transfer

These simulations are computationally expensive for real-time analysis.

### Approach

Developed a multi-stage solver pipeline:

1. Python prototype for model validation
2. High-performance C++ solver
3. Hardware acceleration using **Xilinx Vitis HLS**

### Key results

- Achieved **100× speedup** compared with baseline CPU simulation
- Enabled **real-time reactor emulation**
- Demonstrated CPU–FPGA co-simulation workflow

### Tech stack

C++  
Python  
Scientific computing  
FPGA / Vitis HLS

### Visuals

System architecture and FPGA co-simulation diagrams are included in the repo.

</details>

<details>
<summary><b>Voucher Audit Management System — OCR-based accounting workflow</b></summary>

**Repo**  
https://github.com/yuyao-wang/voucher_audit_management_system_OCR

### Problem

Manual accounting voucher validation is repetitive and error-prone.

Auditors must manually:

- read scanned vouchers
- validate entries
- record approval workflows

### Approach

Designed a **role-based audit workflow system** integrating OCR extraction.

System roles include:

- Auditor
- Voucher checker
- Administrator

### Key features

- OCR-based voucher information extraction
- Role-based approval workflows
- Database-backed document storage
- Web interface for audit operations

### Tech stack

Java  
Spring Boot  
Vue  
MySQL  
OCR APIs

### Artifacts

The repo includes:

- architecture diagrams
- workflow diagrams
- GUI screenshots
- deployment instructions

</details>

<details>
<summary><b>Property Pledge Appraisement ML — collateral valuation</b></summary>

**Repo**  
https://github.com/yuyao-wang/property_pledge_appraisement_ML

### Problem

Banks require reliable valuation models for **real-estate collateral risk assessment**.

### Approach

Constructed a machine learning pipeline using:

- web-scraped housing market data
- macroeconomic indicators
- structured property features

Explored multiple models:

- Random Forest
- XGBoost
- LightGBM
- CatBoost
- Ensemble stacking

### Key results

- Compared model performance across multiple ML algorithms
- Identified important valuation features

### Tech stack

Python  
Scikit-learn  
XGBoost  
LightGBM  
Jupyter notebooks

</details>

<details>
<summary><b>Snakes — data-oriented multiplayer game</b></summary>

**Repo**  
https://github.com/yuyao-wang/Snakes

### Problem

Explore modern **data-oriented game architecture** using ECS.

### Approach

Built a multiplayer snake game engine featuring:

- Entity Component System architecture
- decoupled client-server design
- network communication via ZeroMQ

### Key features

- modular ECS architecture using Flecs
- real-time multiplayer synchronization
- simple graphical rendering with raylib

### Tech stack

C++  
Flecs ECS  
ZeroMQ  
raylib  
CMake

### Run

git clone https://github.com/yuyao-wang/Snakes

cd Snakes
mkdir build && cd build
cmake ..
make

</details>

<details>
<summary><b>LLM Agent — Multi-source tool-calling LLM baselines</b></summary>

**Repo**  
https://github.com/yuyao-wang/LLM-agent

### Problem

Build a practical health-monitoring agent that can handle **temporal, multi-turn tool-calling** across heterogeneous data sources (CGM + event streams).

### Approach

- Built multi-turn function-calling training mixtures for temporal/event-centric supervision
- Structured data in ShareGPT-style tool-call format (`function_call` + `observation` + follow-up reasoning)
- Implemented LoRA/SFT baselines for compact models (Qwen/LLaMA 7B–8B)
- Tracked reproducible run evidence using logs + config snapshots

### Key results / artifacts

- Representative dataset scales:
  - `CGM_event_query_train_set`: 3,912
  - `CGM_time_query_train_set`: 5,053
  - `CGM_merge_query_train_set`: 8,965
  - `dialogue_train_merge`: 14,749
- Baseline run snapshots:
  - Qwen2.5-7B: train loss `0.1533`, eval loss `0.0605`
  - Qwen3-8B (mixture A): train loss `0.3902`, eval loss `0.2737`
  - Qwen3-8B (mixture B): train loss `0.2215`, eval loss `0.0827`

### Tech stack

Python  
PyTorch  
LLM Agents / Tool Calling  
LoRA / SFT  
Qwen / LLaMA  
Distributed Multi-GPU Training  
JSON Data Engineering

### Notes

This repository is presented as a portfolio snapshot of engineering contributions; related paper context is under review.

</details>

## Tech Stack

**ML & AI:** Python · PyTorch · Vision Transformers · Domain Adaptation · LoRA · LLM Agents · Tool Calling · SFT · Qwen · LLaMA  
**Scientific Computing:** C++ · Numerical PDE Solvers · Performance Optimization  
**Remote Sensing:** Sentinel-2 · Landsat · Sentinel-5P · GeoTIFF · NetCDF  
**Systems:** Linux · HPC · Slurm · Git · CMake · Multi-GPU Training  
**Acceleration:** FPGA · Xilinx Vitis HLS



