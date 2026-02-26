# 🏃 Composite Running Blade – Design & FEA Analysis

**CMSA Project – Politecnico di Milano (A.Y. 2024-2025)**  
*Authors:* Gabriele Decortes, **Fabio Marchi**, Emanuele Nicolò Pizzo

---

## 📌 Overview

This project presents the **design and structural optimization** of a **J-shaped composite running blade** for Paralympic sprinting (100 m and 200 m), based on the **Cheetah Xtreme** model by Össur.

Using **Classical Lamination Theory (CLT)** and **Finite Element Analysis (FEA)** in Abaqus/CAE, we optimized the layup configuration to meet:
- ✅ **Structural integrity** (Tsai-Hill criterion, 2000 N load)
- ✅ **Target stiffness** (50 N/mm, max tip displacement 4 cm)
- ✅ **Minimum weight** for enhanced athletic performance

---

## 🔬 Key Results

| Material | Plies | Thickness | Weight | Performance |
|----------|-------|-----------|--------|-------------|
| **CFRP** (Carbon Fiber) | 52 | 1.3 cm | **1.75 kg** | ✅ **Selected** |
| GFRP (Glass Fiber) | 84 | 2.1 cm | 3.5 kg | ❌ Too heavy |
| AA7075 (Aluminum) | – | 1.2 cm | 2.8 kg | ❌ Heavier, prone to corrosion |

**CFRP** was chosen as the optimal material due to its superior **weight-to-stiffness ratio** and **energy return efficiency** (~90%).

---

## 🛠️ Methods

- **CAD modeling:** SolidWorks
- **FEA simulation:** Abaqus/CAE (S4R shell elements, 2140 elements)
- **Manufacturing:** Prepreg-Vacuum Bagging recommended
- **Optimization:** Iterative layup refinement to minimize plies while meeting displacement constraint

---

## 📂 Project Files

- [`CMSA_project__running_blades-1.pdf`](./CMSA_project__running_blades-1.pdf) – Full project report

---

## 📚 References

See full references in the report. Key sources:
- Saleel H. Abood & Majid H. Faidh-Allah (2019) – Analysis of prosthetic running blades
- Yasser Alizadeh (2020) – Dynamic explicit analysis using Abaqus
- Foscan, G. (2021) – Composite materials LCA
