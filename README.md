# 🏃‍♂️ Sprint Running Blade Design  
Finite Element Optimization of Composite vs Aluminium Solutions

## 📖 Overview

This project focuses on the **design and structural optimization of a J-shaped running blade** for short-distance Paralympic sprinting (100–200 m).

The objective was to develop the **lightest possible configuration** capable of:

- Sustaining a **2000 N ground reaction load**
- Limiting tip displacement to **≤ 40 mm** (target stiffness ≈ 50 N/mm)
- Satisfying structural failure criteria

The workflow integrates analytical modelling, composite laminate theory, and nonlinear finite element simulations.

---

## 🎯 Design Strategy

### 1️⃣ Geometry Development
- CAD modelling in *SolidWorks*
- J-shaped profile inspired by elite sprint blades
- Shell-based structural representation

### 2️⃣ Analytical Pre-Assessment
- 2D beam simplification
- Bending moment evaluation
- Identification of the critical curved **“S-region”**

### 3️⃣ Finite Element Implementation (Abaqus/CAE)
- Static General analysis
- Pressure load equivalent to 2000 N
- Encastre boundary condition at socket interface
- Mesh refinement in high-stress areas
- Progressive laminate optimization

Failure criteria used:
- **Tsai–Hill** (composites)
- **Von Mises** (aluminium)

---

## 🧵 Materials Compared

- **CFRP** – Carbon Fiber Reinforced Polymer  
- **GFRP** – Glass Fiber Reinforced Polymer  
- **AA7075** – Aluminium Alloy  

Two symmetric laminate stacking sequences were investigated to evaluate the influence of 90° plies.

---

## 📊 Results Summary

### Structural Integrity (2000 N)

| Material | Plies Required (Failure Safe) |
|----------|------------------------------|
| CFRP     | 28 |
| GFRP     | 44 |

Laminates **without 90° plies** showed improved bending performance.

---

### Displacement Constraint (≤ 40 mm)

| Material | Final Configuration | Weight |
|----------|-------------------|--------|
| CFRP     | 52 plies | 1.75 kg |
| GFRP     | 84 plies | 3.5 kg |
| AA7075   | 1.2 cm thickness | 2.8 kg |

---

## 🏆 Final Outcome

**CFRP was selected** as the optimal solution due to:

- Superior stiffness-to-weight ratio  
- Lower inertial mass  
- Compliance with both failure and displacement targets  

Although aluminium satisfies structural constraints, it results in higher mass and lower sprint performance efficiency.

---

## 🏭 Manufacturing Considerations

Selected process:

- ✅ **Prepreg Vacuum Bagging**

Reasons:
- Accurate fiber orientation control  
- Reduced variability  
- Industrial scalability for customized prosthetics  

---

## 🛠 Tools & Engineering Framework

- SolidWorks – CAD modelling  
- Abaqus/CAE – Finite Element Analysis  
- Classical Lamination Theory (CLT)  
- Composite failure modelling (Tsai–Hill)

---

## 📌 Key Engineering Takeaways

- The curved region governs structural behaviour.  
- 90° plies are detrimental under dominant bending loads.  
- Weight reduction is the primary performance driver.  
- CFRP clearly outperforms GFRP and aluminium for sprint-specific prosthetic applications.
