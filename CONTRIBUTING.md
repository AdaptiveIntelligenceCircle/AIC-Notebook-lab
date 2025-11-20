# Contributing Guide — AIC-Lab

Thank you for your interest in contributing to AIC-Lab!

This project serves as a scientific laboratory for the Adaptive Intelligence ecosystem, so your technical contributions will help make the system better and more transparent.

## 1. How to contribute

### 1.1. Getting started
- Fork the repo and clone it.

- Create a new branch from `main`.

For example: git checkout -b feature/my-improvement

### 1.2. Pull Request (PR)
PR must ensure:
- clearly describe the change,
- attach test results (if any),
- do not break backward compatibility,
- comply with the Code of Conduct.

Template PR:

- Summary

(Details you changed)

- Motivation

(Why this change is needed)

- Tests

(Notebooks / code with evidence)

- Impact

(Impact on other modules)

---

## 2. Code Rules

### 2.1. Python
- PEP8
- Do not create global state unless clearly stated
- Always have type hints

### 2.2. C++
- Comply with C++23
- Do not use raw pointers where smart pointers are available
- Separate header/source
- Do not use broad namespaces (`using namespace std;`)

---

## 3. Notebook Standards

### 3.1. Notebooks must have:
- clear goal (Objective)
- pipeline description
- simulation results
- “Insights & Interpretation” section

### 3.2. Do not commit:
- `.ipynb_checkpoints` file
- large output
- sensitive data

---

## 4. Areas you can contribute

### 🔹 Simulation
- behavior simulation
- packet pipeline

### 🔹 Visualization
- flow graph
- anomaly map

### 🔹 C++
- performance tuning
- state machine engine

### 🔹 Documentation
- wiki addition
- module tutorial writing

---

## 5. Review process

- Review focuses on logic, not personal bias.
- Reviewers have the right to request additional benchmarks or simulations.
- Do not merge when the test fails.

---

Thank you for helping AIC-Lab develop sustainably and responsibly!