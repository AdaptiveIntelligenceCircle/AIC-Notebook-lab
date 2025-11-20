# 🚀 **RELEASE_PROCESS.md**

# AIC Release Process

AIC follows a predictable but security-focused release workflow.

---

## Release Types

### **1. Patch Release (`vX.Y.Z`)**

* Bug fixes
* Documentation updates
* Small improvements
* No breaking changes

### **2. Minor Release (`vX.Y.0`)**

* New modules
* New APIs
* Backwards-compatible improvements

### **3. Major Release (`vX.0.0`)**

* Breaking API changes
* Large architectural changes
* Security model updates

---

## Release Workflow

### **Step 1 — Proposal**

Opened as:

* GitHub Issue + `release-proposal` tag
* Must describe:

  * Changes
  * Compatibility impact
  * Security implications
  * Migration notes

### **Step 2 — Development**

* PR must target `dev` branch.
* All new modules require:

  * Unit tests
  * Integration tests
  * Security review
  * Architecture review

### **Step 3 — Review**

* Code review by module maintainers
* Security review by core maintainers
* Documentation review

### **Step 4 — Pre-Release**

* Create tag: `vX.Y.Z-rc1`
* Run:

  * Simulation tests
  * Introspection stability tests
  * Rollback behavior tests
  * Plugin compatibility checks
* Publish to GitHub releases (prerelease)

### **Step 5 — Final Release**

* Merge to `main`
* Tag: `vX.Y.Z`
* Publish:

  * Release notes
  * Migration guide (if needed)
  * Updated architecture diagrams

---

## Hotfix Policy

* Only for critical security issues
* Must bypass normal feature reviews
* Requires unanimous maintainer approval

---

## End-of-Life Policy

* Minor versions supported for 18 months
* Major versions supported for 3 years
* Security-critical core receives extended support

---
