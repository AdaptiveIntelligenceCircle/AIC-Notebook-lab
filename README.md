# 🧪 **AIC-Lab: Adaptive Intelligence Laboratory**

*A research & simulation environment for the Adaptive Intelligence Circle (AIC) ecosystem.*
AIC-Lab provides a visual sandbox for simulating, testing, and analyzing components of the AIC system, including packet pipeline, preprocessing, anomaly detection, introspection, behavior engine, and rollback logic — visualized using Jupyter Notebook and Google Colab.

This repository is designed to run in parallel with **AIC Core (C++23)** and serve as an **algorithm development lab**, enabling you to quickly test, simulate complex behavior, and experiment with ideas before deploying them to production systems.

---

# 📌 **AIC-Lab Goals**

AIC-Lab was created to serve 5 main goals:

### ✅ 1) **Fast testing & simulation using Notebook**

* simulation pipeline from **sensor → preprocessing → protection → rollback**
* random packet generation, simulated attacks, error data
* analysis of internal system behavior and state

### ✅ 2) **Introspection & Behavior Engine Simulation**

* introspection logic testing
* modeling behavior, reactions, confidence scores
* observing event statistics and rollback mechanisms

### ✅ 3) **Parallel comparison Python ↔ C++**

Run the same logic:

* `generate_packet.py`
* `generate_packet.cpp`

→ Cross-validate to check consistency, logic, and performance.

### ✅ 4) **Visualization**

Helps see the whole picture of AIC operations:

* timing diagram
* state transition
* magnitude of anomaly
* heatmap for event pipeline

### ✅ 5) **Performance Benchmark**

Record:

* packet processing time
* rollback latency
* throughput preprocessing
* introspection speed
From there, optimize Core C++.

---

# 📂 **Folder structure**

```
AIC-Lab/
│
├── notebooks/
│ ├── 01_intro.ipynb
│ ├── 02_generate_packet_test.ipynb
│ ├── 03_behavior_simulation.ipynb
│ ├── 04_anomaly_injection.ipynb
│ ├── 05_rollback_simulation.ipynb
│ ├── 06_cross_validation_cpp_python.ipynb
│ ├── 07_remote_slm_plugin_test.ipynb
│ └── 08_introspection_engine.ipynb
│
├── cpp/
│ ├── CMakeLists.txt
│ ├── aic_core_minimal.cpp
│ ├── generate_packet.cpp
│ ├── simulate_behavior.cpp
│ └── packet.h
│
├── python/
│ ├── generate_packet.py
│ ├── behavior_engine_sim.py
│ ├── preprocessing_sim.py
│ ├── introspection_sim.py
│ └── utils.py
│
├── data/
│ ├── test_packets.json
│ ├── anomaly_cases.json
│ └── behavior_rules.json
│
├── colab_setup.sh
└── README.md
```

---

# 🚀 **Getting Started**

## ▶ 1. Use on Windows + VSCode

Install extensions:

* **Python**
* **Jupyter**
* **CMake Tools**
* **C/C++**

Run Notebook directly in VSCode.

## ▶ 2. Using Google Colab

Run any notebook → will automatically install:

```bash
!bash colab_setup.sh
```

Includes:

* g++
* cmake
* build C++ scripts
* Python environment

## ▶ 3. Build C++ directly in Notebook

Example in Colab:

```bash
%cd cpp
!cmake .
!make
!./aic_core_minimal
```

---

# 🛠 **Main components**

## **1. Packet Simulation**

🧩 Create packet:

* timestamp
* payload
* entropy
* magnitude
* actor ID
* anomaly level

Ensure Python ↔ C++ logic is consistent through cross-testing.

---

## **2. Behavior Engine Simulation**

📘 Simulation:

* rules
* states
* actions
* adaptive responses
* warning levels

Notebook helps visualize the entire lifecycle of a behavior.

---

## **3. Introspection Simulation**

🔍 Test:

* `analyzeThoughtProcess`
* `summarizeIntrospection`
* `memory snapshot`
* `reasoning tree`
* `self-evaluation score`

---

## **4. Rollback Simulation**

🔥 Simulate the situation:

* overload
* anomaly
* misbehavior
* policy violation
→ Then observe the process **rollback → stabilize → recover**.

---

## **5. Preprocessing Simulation**

🧼 Simulation:

* data cleaner
* feature extractor
* entropy filters
* windowed statistics

---

# 📊 **Visualization Examples**

Repo supports exporting:

* anomaly graph over time
* behavior graph
* sensor value histogram
* flow graph pipeline
* ​​checkpoint timeline of rollback

---

# 🔗 **Connect to AIC-Core**

AIC-Lab **does** not replace AIC-Core.

It only serves as:

🧪 *Research lab*
📈 *Simulation sandbox*
🔍 *Introspection & validation tool*
🚦 *Development acceleration test suite*

All the actual C++ is still in AIC-Core.

---

# 🧭 Roadmap

## **v0.1 — Base Notebooks**

* packet simulation
* anomaly injection
* cross test Python ↔ C++

## **v0.2 — Behavior Engine Simulation**

* rule-based simulation
* visualize state machine

## **v0.3 — Introspection Engine**

* inference modeling
* reasoning tree flow

## **v0.4 — Rollback Mechanism**

* hybrid rollback
* consistency check
* log timeline

## **v1.0 — Full System Simulation**

* end-to-end sensor → rollback
* unified interface
* visualization toolkit

---

# 🤝 Contribute

Anyone who wants to:

* simulate behavior
* design new plugins
* write demonstration notebooks
* test anomaly

AIC-Lab is open.

---

# 🧘 AIC-Lab Philosophy

**“Who can also see a system working through code.

But very few people get to see inside it:
its thinking, behavior, adaptation, and self-protection mechanisms.”**

AIC-Lab was born to open that door.