# Yuyao (Phoebe) Wang

![MSc ECE @ University of Alberta](https://img.shields.io/badge/MSc%20ECE-University%20of%20Alberta-informational)
![Focus: Multimodal ML](https://img.shields.io/badge/Focus-Multimodal%20ML-blue)
![Focus: Geospatial AI](https://img.shields.io/badge/Focus-Geospatial%20AI-blue)
![Focus: Applied AI Systems](https://img.shields.io/badge/Focus-Applied%20AI%20Systems-blue)
![Python](https://img.shields.io/badge/Code-Python-3776AB?logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/ML-PyTorch-EE4C2C?logo=pytorch&logoColor=white)
![C++](https://img.shields.io/badge/Code-C%2B%2B-00599C?logo=c%2B%2B&logoColor=white)

**Machine Learning Engineer focused on multimodal ML, geospatial AI, and applied AI systems.**  
MSc Electrical & Computer Engineering @ University of Alberta.

I build machine learning systems that connect real-world data, model adaptation, and practical engineering workflows — from multi-sensor satellite methane detection to browser-based AI automation and scientific simulation systems.

**Open to:** Machine Learning Engineer · Applied AI Engineer · Software Engineer, ML Systems

**Quick links:**  
[Email](mailto:yuyaow42@gmail.com) · [LinkedIn](https://linkedin.com/in/yuyao-wang) · [GitHub](https://github.com/yuyao-wang)

---

## About Me

My interests lie at the intersection of **machine learning**, **geospatial / remote sensing data engineering**, and **applied AI systems**.

Across my projects, I often work with real-world constraints such as incomplete observations, cross-domain mismatch, noisy labels, limited data availability, and deployment-oriented engineering trade-offs. I am especially interested in building ML systems that are not only accurate in controlled settings, but also practical under real data and workflow constraints.

Current areas I am exploring include:

- Multimodal ML with incomplete or heterogeneous real-world data
- Vision Transformer-based modeling, adaptation, and evaluation
- LLM agents, tool-calling workflows, and applied AI automation
- Data engineering pipelines for ML experiments and reproducible evaluation
- Performance-aware implementation with Python, C++, and distributed / HPC workflows

---

## Featured Projects

<details>
<summary><b>MethaneFuse — Multi-Sensor Satellite Methane Detection</b></summary>

**Repo:**  
https://github.com/yuyao-wang/MethaneFuse

### Problem

Methane plume observations are sparse, transient, and sensor-dependent. A single satellite sensor is often limited by revisit time, cloud cover, spatial resolution, spectral coverage, and acquisition quality.

This project explores methane plume detection from **partially available multi-sensor satellite observations**, where different events may have different combinations of available sensor data.

### Approach

- Built an event-centered multi-sensor learning pipeline using satellite observations from different sensor domains.
- Developed Vision Transformer-based modeling components for methane plume detection under missing-sensor and cross-sensor conditions.
- Worked on dataset construction, sensor matching, quality filtering, model evaluation, and research reporting.
- Designed the project as a public-safe portfolio snapshot while withholding full datasets, checkpoints, and unpublished experimental details.

### Public-safe artifacts

The public repo includes demo components such as:

- EMIT-like hyperspectral to multispectral bandpass simulation
- Domain-adaptive ViT-style adapter demo using synthetic tensors
- Portfolio-level documentation of the multi-sensor methane detection workflow

### Tech stack

Python · PyTorch · Vision Transformers · Remote Sensing · Geospatial ML · Domain Adaptation

### Demo

```bash
python3 portfolio/demo/emit_bandpass_simulation_demo.py
python3 portfolio/demo/multidomain_vit_adapter_demo.py
```

</details>

---

<details>
<summary><b>Hanzi Browse — Open-Source Browser Agent Infrastructure</b></summary>

**Repo:**  
https://github.com/hanzili/hanzi-browse

### Problem

Browser agents need reliable ways to interact with real websites. Generic web automation often fails when websites have complex UI flows, dynamic content, or site-specific interaction patterns.

### Contribution

Contributed to an open-source browser automation project that helps AI agents interact with real websites using site-specific playbooks.

### Work involved

- Contributed to an agent-facing browser automation workflow.
- Worked with real-world web interaction patterns and product-facing AI tooling.
- Practiced collaborative open-source development through issue-driven implementation and code review.
- Gained experience with practical AI agent infrastructure beyond isolated model training.

### Tech stack

JavaScript / TypeScript · Browser Automation · AI Agents · MCP · Open Source

</details>

---

<details>
<summary><b>MSRE-BC-1D — Real-Time Multiphysics Reactor Simulation</b></summary>

**Repo:**  
https://github.com/yuyao-wang/MSRE-BC-1D

### Problem

Molten salt reactor dynamics involve stiff and coupled physical processes, including neutron diffusion, delayed neutron kinetics, thermal hydraulics, and heat transfer.

These simulations are computationally expensive and difficult to run in real time.

### Approach

Developed a multi-stage scientific computing workflow:

1. Python prototype for model validation and experimentation
2. C++ implementation for performance-oriented simulation
3. Hardware-aware implementation exploration using Xilinx Vitis HLS

### Key work

- Built Python and C++ simulation components for coupled neutron diffusion, delayed neutron kinetics, and thermal-hydraulics models.
- Converted simulation workflows from Python prototypes to C++ implementations for improved performance and hardware-oriented development.
- Explored CPU–FPGA co-simulation and acceleration-oriented implementation for real-time simulation.

### Tech stack

C++ · Python · Numerical PDEs · Scientific Computing · HPC · Vitis HLS

</details>

---

## Research and Collaboration Experience

<details>
<summary><b>LLM Agent — Multi-Source Tool-Calling LLM Baselines</b></summary>

**Repo:**  
https://github.com/yuyao-wang/LLM-agent

### Context

This repository is presented as a portfolio snapshot of research assistance and experimental engineering work related to temporal, multi-turn LLM agent workflows over heterogeneous data sources.

It is not presented as my independent project.

### Work involved

- Worked with multi-turn tool-calling data formats involving function calls, observations, and follow-up reasoning.
- Implemented and organized LoRA / SFT baseline experiments for compact LLMs.
- Prepared reproducible experiment evidence, training configurations, logs, and dataset-scale summaries.
- Organized data and training artifacts for agent-oriented model evaluation.

### Tech stack

Python · PyTorch · Hugging Face · LoRA / SFT · LLM Agents · Tool Calling · Multi-GPU Training · JSON Data Engineering

</details>

---

## Earlier Projects

<details>
<summary><b>Voucher Audit Management System — OCR-Based Accounting Workflow</b></summary>

**Repo:**  
https://github.com/yuyao-wang/voucher_audit_management_system_OCR

### Problem

Manual accounting voucher validation is repetitive and error-prone. Auditors need to read scanned vouchers, validate entries, and record approval workflows.

### Approach

Designed a role-based audit workflow system integrating OCR extraction and database-backed document management.

### Key features

- OCR-based voucher information extraction
- Role-based approval workflows
- Database-backed document storage
- Web interface for audit operations
- Architecture diagrams, workflow diagrams, GUI screenshots, and deployment documentation

### Tech stack

Java · Spring Boot · Vue · MySQL · OCR APIs

</details>

---

<details>
<summary><b>Property Pledge Appraisement ML — Collateral Valuation</b></summary>

**Repo:**  
https://github.com/yuyao-wang/property_pledge_appraisement_ML

### Problem

Banks require reliable valuation models for real-estate collateral risk assessment.

### Approach

Constructed a machine learning pipeline using structured property data, housing market information, and macroeconomic indicators.

### Work involved

- Built tabular ML pipelines for property valuation.
- Compared multiple machine learning models, including Random Forest, XGBoost, LightGBM, CatBoost, and ensemble methods.
- Worked on feature engineering, model evaluation, and finance-oriented risk assessment.

### Tech stack

Python · Scikit-learn · XGBoost · LightGBM · CatBoost · Jupyter Notebooks

</details>

---

<details>
<summary><b>Snakes — Data-Oriented Multiplayer Game</b></summary>

**Repo:**  
https://github.com/yuyao-wang/Snakes

### Problem

Explore modern data-oriented game architecture using ECS and networked multiplayer design.

### Approach

Built a multiplayer snake game engine featuring:

- Entity Component System architecture
- Decoupled client-server design
- Network communication via ZeroMQ
- Simple graphical rendering with raylib

### Tech stack

C++ · Flecs ECS · ZeroMQ · raylib · CMake

### Run

```bash
git clone https://github.com/yuyao-wang/Snakes
cd Snakes
mkdir build && cd build
cmake ..
make
```

</details>

---

## Technical Skills

**Core ML:** Python · PyTorch · Hugging Face Transformers · Vision Transformers · LoRA / SFT · Multimodal Learning · Model Fine-tuning · Model Evaluation

**LLM & Agent Systems:** Tool Calling · Multi-turn Agent Data · Function-calling Workflows · Browser Automation · MCP · JSON Data Pipelines

**Data & Experiment Engineering:** NumPy · Pandas · Jupyter · Dataset Construction · Data Preprocessing · Experiment Logging · Reproducible Training

**Software Engineering:** C++ · JavaScript / TypeScript · Java · SQL · Bash · Git · Linux · CMake · Node.js · REST APIs

**Geospatial & Scientific Computing:** Satellite Imagery · Multi-sensor Data Processing · GeoTIFF · NetCDF · Google Earth Engine · Slurm / HPC · Vitis HLS

---

## Contact

I am interested in applied AI systems, geospatial AI, and research-to-product ML workflows.

Feel free to reach out through [LinkedIn](https://linkedin.com/in/yuyao-wang) or email me at [yuyaow42@gmail.com](mailto:yuyaow42@gmail.com).
