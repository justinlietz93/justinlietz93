<!-- Profile README for @JUSTIN_GH_HANDLE -->
<h1 align="center">Void Dynamics Model (VDM)</h1>
<p align="center">
  A real-time, event-driven, reaction–diffusion substrate with walker ecology & memory steering.  
  <br/>No dense scans. No epoch training. Constraint satisfaction in the moment.
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

### 🔭 What I’m building
- **VDM Core** — reaction–diffusion field + walker ecology + scoreboard/GDSP gating  
- **Memory Steering** — dynamic knowledge graph with event-driven updates  
- **Real-time control** — swap massive pretraining for fast constraint satisfaction

**Reproducibility:** baselines + QA artifacts are archived on Zenodo. Code lives in public GitHub repos with tests and docs.

---

### 📦 Repositories (pin these)
- **Prometheus_Void-Dynamics_Model** → core substrate, walkers, scoreboard  
- **Modular_Utilities** → local tooling, scripts, AMD/ROCm helpers  
- **agent_tools** → orchestration, validators, critics, routers

> Tip: Pin them via “Customize profile” so they appear above the fold.

---

### 🧪 Reproducible records (Zenodo)
- **A Logarithmic First Integral for the Logistic On-Site Law in Void Dynamics**  
  DOI: **10.5281/zenodo.XXXXXXXX**  
- **RD baselines, convergence, Q-drift, front speed** (datasets + figures)  
  See my Zenodo author page: **https://zenodo.org/records/?q=creator%3A%22Lietz%2C%20Justin%22** *(or your direct profile link)*

> Use your **concept DOI** in badges if you want a stable “latest” link. Version DOIs point to a specific release.

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
