# Security Policy — AIC-Lab

AIC-Lab is a research project related to adaptive system simulation, introspection engine and protection pipeline. Therefore, the security of the source code and simulation environment is a top priority.

## 1. Report a vulnerability

If you discover a security issue:

### Please send an email directly to:
**aic-security@protonmail.com (example)**

In the email, please describe:
- how to reproduce the bug,
- potential impact,
- related files,
- temporary solution (if any).

**Absolutely do not create a public issue when the bug can cause risks.**

---

## 2. What is the scope?

### Covered:
- simulation engine C++ code
- packet generator
- introspection logic
- behavior rules
- Python utilities
- pipeline visualization scripts

### Not covered:
- AIC Core (managed in another repo)
- third-party dependencies
- notebook output

---

## 3. Project security principles

### 3.1. Do not include dangerous payloads
- malware
- shell injection
- backdoor
- exploit demo in production code

If you need to simulate an attack → use **anomaly simulation** safely.

### 3.2. Do not use personal keys/tokens
- API keys
- private endpoint
- internal URL

### 3.3. Ensure sandbox
Notebook only simulates, does not interfere with real systems.

---

## 4. Vulnerability Handling Process

1. Receive report via email
2. Confirm within 72 hours
3. Classify the level
4. Fix the error within:
- high level: 72 hours
- medium level: 7 days
- low level: 14 days
5. Public announcement after patching

---

## 5. AIC-Lab's security philosophy

AIC-Lab prioritizes:
- transparency
- honesty
- academic nature
- fast fix, no blame

The more transparent the system → the harder it is to exploit → the more trustworthy.