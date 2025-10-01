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
  <!-- LICENSE -->
  <a href="https://github.com/Neuroca-Inc/Prometheus_Void-Dynamics_Model/blob/main/LICENSE.md"><img src="https://img.shields.io/badge/Academic%2FCommercial%20Dual-License?label=LICENSE&color=%23fff200&link=https%3A%2F%2Fgithub.com%2FNeuroca-Inc%2FPrometheus_Void-Dynamics_Model%2Fblob%2Fmain%2FLICENSE.md" alt="Dual Academic/Commercial License"></a>
</p>

---

<img width="800" height="800" alt="image" src="https://github.com/user-attachments/assets/7ee95b3a-75a3-48bd-a003-a13c7e5ed845" />

---

### 🔭 What I’m building
- **VDM** — reaction–diffusion field intelligence + walker ecology + scoreboard/GDSP gating  
- **Memory Steering** — dynamic knowledge graph with event-driven updates  
- **Real-time control** — swap massive pretraining for fast constraint satisfaction

**Reproducibility:** baselines + QA artifacts are archived on Zenodo. Code lives in public GitHub repos with tests and docs.

---

### 🧪 Reproducible records (Zenodo)
- Latest Zenodo Upload: **[A Logarithmic First Integral for the Logistic On Site Law in Void Dynamics
](https://zenodo.org/records/17220869?token=eyJhbGciOiJIUzUxMiJ9.eyJpZCI6Ijg5NzU0YWVkLTk4OTktNDkzMC1hMDQ4LTEwYThmMjMwYmY5MyIsImRhdGEiOnt9LCJyYW5kb20iOiJjYTg4YjhhZmJmZGVkMmIyMTFkNmEzOWIzNmFkMDk2NCJ9.ACynGDMzx4lAtPOfNNX-vDPPh8DMEISWTOoCO-I3DJ9aktZ_RZCDm0uUwxtVi5eVYbsrMopwcANKznI8WrslbQ)**
- DOI: **10.5281/zenodo.17220869**  
- **RD baselines, convergence, Q-drift, front speed** (datasets + figures)  

---

### ⚙️ Quickstart
```bash
# clone
git clone https://github.com/Neuroca-Inc/Prometheus_Void-Dynamics_Model.git
cd Prometheus_Void-Dynamics_Model

# create env (exact commands in repo README)
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

# run a Reaction Diffusion + walkers with Memory Steering demo (Coming soon)

# Otherwise check out the src/ folder for the available public sims
```

### 🗺️ Roadmap (Oct~Dec 2025)
- Notebook mirrors of each test ✅
- 100% Reproducible, falsifiable claims ✅
- Currently working real time model ✅
- Zero training ✅
- Online causality based learning
- Physics driven intelligence model ✅

**CURRENT Execution model:** All tests live in `src/{domain name}/`, figures appear in `figures/{domain name}` if passing and `figures/{domain name}/failed_runs/` if failed. The same goes for logs, just replace `figures/` with `logs/` in the file path to find them.

**GOAL Execution model:** All tests live in `notebooks/`, render figures + filepaths inline, and write results under `artifacts/`. A master notebook runs the full suite with clear explanations and emits a manifest.

```bash
# Run-all (executes the full suite and saves executed copy)
jupyter nbconvert --to notebook --execute notebooks/00_RUN_ALL.ipynb --output notebooks/00_RUN_ALL.out.ipynb
```

**Future Layout**

```
notebooks/
  00_RUN_ALL.ipynb
  01_rd_front_speed.ipynb
  02_rd_dispersion.ipynb
  03_invariant_drift.ipynb
  10_walkers_min_demo.ipynb
  11_locality_bounds.ipynb
  12_gdsp_budget_sweeps.ipynb
  20_memsteer_acceptance.ipynb
  30_rt_control_slice.ipynb
artifacts/
  rd/ walkers/ memsteer/ control/ meta/
```

**Current Status legend:** `PROVEN` (axiom gates passed) · `PLAUSIBLE` (design + prelim data) · `NEEDS_DATA` (tests pending)
**Hardware:** I use AMD/ROCm only (MI100, 7900 XTX). CPU fallbacks use smaller grids. I easily ran 100,000 neurons on battery power using an Acer Aspire notebook, planning to achieve 1 billion neurons on the bigger machine.

#### October 2025 (Weeks 1–4)

* [DONE] **RD Baselines v0.2** — `01_rd_front_speed`, `02_rd_dispersion`, `03_invariant_drift` → `artifacts/rd/` (`PROVEN`)
  Gates: front-speed R² ≥ **0.9999**, rel-err ≤ **5%**; dispersion median rel-err ≤ **1e-1**, array R² ≥ **0.98**; on-site invariant drift ≤ **1e-8/step**.
* [DONE] **Minimal Walkers + GDSP** — `10_walkers_min_demo`, `11_locality_bounds`, `12_gdsp_budget_sweeps` → `artifacts/walkers/`, `artifacts/meta/telemetry.json` (`PROVEN`)
  Gates: finite-support growth within bound; **no dense scans**; GDSP budget never oversubscribed; event telemetry saved.
* [STARTED] **Memory Steering v0.1** — `20_memsteer_acceptance` → `artifacts/memsteer/` (`PLAUSIBLE`)
  Gates: retention half-life = setpoint ± **10%**; steering latency < **2×** baseline RD horizon; interference curve monotone with steer strength.

#### November 2025 (Weeks 1–4) — **v1.0 “model finished”**

* [STARTED] **Real-Time Control Slice** — `30_rt_control_slice` → `artifacts/control/` (`PLAUSIBLE→PROVEN`)
  Gates: goal attainment ≥ **90%** (N seeds); control energy ≤ baseline; perturbation recovery ≤ **2×** unperturbed horizon.
  ***`The model is currently capable of post-graduate level reasoning on human readable casuality exams.`***
* [STARTED] **Release v1.0 Priority Pack** — produced by `00_RUN_ALL.ipynb`
  Outputs: executed `00_RUN_ALL.out.ipynb`, figures, CSV/JSON metrics, seeds, and `artifacts/meta/manifest.json` bundled to `artifacts/v1.0_priority_pack/`.

**Provenance & checks (written by `00_RUN_ALL.ipynb`)**

* Manifest: `artifacts/meta/manifest.json` (paths to all outputs).
* Contradiction report on failure: `artifacts/meta/CONTRADICTION_REPORT.json` (which gate failed + notebook cell refs).
