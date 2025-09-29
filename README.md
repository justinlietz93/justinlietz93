<!-- Profile README for @JUSTIN_GH_HANDLE -->
<h1 align="center">Void Dynamics Model (VDM)</h1>
<p align="center">
  A real-time, event-driven, reaction–diffusion substrate with void walker ecology & memory steering.  
  <br/>No dense scans. Zero training. Divergent reasoning. Constraint satisfaction in the moment.
</p>

<p align="center">
  <!-- Zenodo badge: use your version DOI or concept DOI for “latest” -->
  <a href="https://doi.org/10.5281/zenodo.17220869"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.17220869.svg" alt="DOI"></a>
  <!-- ORCID badge (optional) -->
  <a href="https://orcid.org/0009-0008-9028-1366"><img src="https://img.shields.io/badge/ORCID-0009--0008--9028--1366-blue?style=flat-square" alt="ORCID"></a>
  <!-- AMD/ROCm stance -->
  <img src="https://img.shields.io/badge/GPU-AMD%2FROCm-only?style=flat-square" alt="AMD/ROCm only">
  <!-- License badge -->
  <img src="https://img.shields.io/badge/License-Apache--2.0-informational?style=flat-square" alt="License">
</p>

---

<img width="800" height="800" alt="image" src="https://github.com/user-attachments/assets/7ee95b3a-75a3-48bd-a003-a13c7e5ed845" />

---

### 🔭 What I’m building
- **VDM** — reaction–diffusion field + walker ecology + scoreboard/GDSP gating  
- **Memory Steering** — dynamic knowledge graph with event-driven updates  
- **Real-time control** — swap massive pretraining for fast constraint satisfaction

**Reproducibility:** baselines + QA artifacts are archived on Zenodo. Code lives in public GitHub repos with tests and docs.

---

### 📦 Repositories (pinned below)
- **Prometheus_Void-Dynamics_Model** → substrate, walkers, scoreboard  
- **Modular_Utilities** → local tooling, scripts, AMD/ROCm helpers  
- **agent_tools** → orchestration, validators, critics, routers

---

### 🧪 Reproducible records (Zenodo)
- Latest Zenodo Upload: **[A Logarithmic First Integral for the Logistic On Site Law in Void Dynamics
](https://zenodo.org/records/17220869?token=eyJhbGciOiJIUzUxMiJ9.eyJpZCI6Ijg5NzU0YWVkLTk4OTktNDkzMC1hMDQ4LTEwYThmMjMwYmY5MyIsImRhdGEiOnt9LCJyYW5kb20iOiJjYTg4YjhhZmJmZGVkMmIyMTFkNmEzOWIzNmFkMDk2NCJ9.ACynGDMzx4lAtPOfNNX-vDPPh8DMEISWTOoCO-I3DJ9aktZ_RZCDm0uUwxtVi5eVYbsrMopwcANKznI8WrslbQ)**
- DOI: **10.5281/zenodo.17220869**  
- **RD baselines, convergence, Q-drift, front speed** (datasets + figures)  

---

### ⚙️ Quickstart (local, AMD/ROCm)
```bash
# clone
git clone https://github.com/JUSTIN_ORG/Prometheus_Void-Dynamics_Model.git
cd Prometheus_Void-Dynamics_Model

# create env (exact commands in repo README)
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

# run a minimal RD + walkers demo
python demos/minimal_vdm.py  # produces figures, logs, and a short report
