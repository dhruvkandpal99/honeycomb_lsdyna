# 📄 Blast-Induced High Strain Rate Crushing of Honeycomb (Accurate Shell Mesh) — LS-DYNA

## 📌 Overview
This repository contains a replication of the paper:  
**"Blast-Induced Compression of a Thin-Walled
Aluminum Honeycomb Structure—Experiment
and Modeling"**  
by Magda Stanczak et al., published in Metals, 2019.  

The objective is to reproduce the main results using LS-DYNA and provide clean input decks and output files for verification and further study.

Read my blog for details: [my blog!](https://dhruvkandpal99.github.io/posts/mypost/)

---

## ⚙️ Contents
- ✅ LS-DYNA input files (`.k` files)
- ✅ Results (crush simulation, response Force-Time plot)
- ✅ CSV files of Force-Time curves (generated using https://plotdigitizer.com/app)
- ✅ Comparision (jupyter notebooks)

---

## 🔑 Main Objectives
- Simulate the response of a 53-cell aluminum honeycomb under an EDST-induced blast load.
- Use an accurate geometry-based shell mesh to capture realistic deformation. [Click here to see the procedure.](https://youtu.be/dm4S_Yn3YtE?feature=shared)
- **Validate key results:**  
  - Response **Force-Time curve**
  - Final crushed height of the honeycomb.
- Provide a reusable LS-DYNA input deck for blast-induced high strain rate studies.

---

## 🚀 How to Run
1. **Requirements:**  
   - LS-DYNA version: LS-Run 2022 R1  
   - LS-Prepost 4.7.7
   - Python 3+
   - Jupyter Notebooks

2. **Run simulation:**  
   - Open the keyword (.k) file in LS-Prepost. 
   - Click on File> Run LS-DYNA
   - Run the simulation in LS-RUN with double precision 

\* In LS-Prepost, click on Keywrd tab> CONTROL> TIMESTEP, then change the TSSFAC to 0.0001, this would ensure accurate results but can take upto 2 days to run on workstation

---

## 📊 Expected Results
- d3plot, rcforc (drag the d3plot file into the LS-Prepost window to visualize the results)
- Final Simulation (d3plot):

https://github.com/user-attachments/assets/0d0790d2-4542-401b-b07f-d53abd668625

  
  
  - Force Response (mN) vs time (ms) -- rcforc:
<img src="https://github.com/user-attachments/assets/276416be-9150-4db9-859a-f8aaeebc72df" alt="forceVtime_simulated" width="500">

  - Final Crushed Height:
<img width="500" alt="Screenshot 2025-06-21 at 4 03 37 PM" src="https://github.com/user-attachments/assets/cc9cc956-40f5-4fb3-b266-ab6c590878b7" />

---


## ✅ Validation

- Using Jupyter Notebook (python)
<img src = "https://github.com/user-attachments/assets/b0fe2ad5-fe2e-4e6c-896b-8babf67842d8" alt="forceVtimeComparision" width ="500">
  
*Figure: Force (mN) vs time (ms) Comparision of True and Simulation values -- RMSE = 0.1895 (i.e., 18.95%)*


- Final Crushed Height (as per paper)
  
<img width="600" alt="Screenshot 2025-06-21 at 4 16 21 PM" src="https://github.com/user-attachments/assets/ca1dca2e-d32e-4204-86f2-987d1332b1f4" />

*Figure: Subsequent frames depicting compression of the honeycomb (as per paper)*

---

## 📚References

Stanczak M, Fras T, Blanc L, Pawlowski P, Rusinek A. Blast-Induced Compression of a Thin-Walled Aluminum Honeycomb Structure—Experiment and Modeling. Metals. 2019; 9(12):1350. https://doi.org/10.3390/met9121350

---

## 📄 Licence 
This project is licensed under MIT License
