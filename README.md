# 📄 Blast-Induced High Strain Rate Crushing of Honeycomb (Accurate Shell Mesh) — LS-DYNA

## 📌 Overview
This repository contains a replication of the paper:  
**"Blast-Induced Compression of a Thin-Walled
Aluminum Honeycomb Structure—Experiment
and Modeling"**  
by Magda Stanczak et al., published in Metals, 2019.  

The objective is to reproduce the main results using LS-DYNA and provide clean input decks and output files for verification and further study.

---

## ⚙️ Contents
- ✅ LS-DYNA input files (`.k` files)
- ✅ Results (crush simulation, response Force-Time plot)
- ✅ Comparision (jupyter notebooks)
- ✅ Detailed report ([report.pdf](report.pdf))

---

## 🔑 Main Objectives
- Simulate the response of a 53-cell aluminum honeycomb under an EDST-induced blast load.
- Use an accurate geometry-based shell mesh to capture realistic deformation.
- **Validate key results:**  
  - Response **Force-Time curve**
  - Final crushed height of the honeycomb.
- Provide a reusable LS-DYNA input deck for blast-induced high strain rate studies.

---

## 🚀 How to Run
1. **Requirements:**  
   - LS-DYNA version: LS-Run 2022 R1  
   - LS-Prepost 4.7.7 

2. **Run simulation:**  
   - Open the keyword (.k) file in LS-Prepost. 
   - Click on File> Run LS-DYNA
   - Run the simulation in LS-RUN with double precision 

\* In LS-Prepost, click on Keywrd tab> CONTROL> TIMESTEP, then change the TSSFAC to 0.0001, this would ensure accurate results but can take upto 2 days to run on workstation

## 📊 Expected Results
- d3plot, rcforc (drag the d3plot file into the LS-Prepost window to visualize the results)
- Final Simulation and Plots:

https://github.com/user-attachments/assets/0d0790d2-4542-401b-b07f-d53abd668625

