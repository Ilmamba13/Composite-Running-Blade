Sprint Running Blade – Design & FEM Optimization

Design and structural optimization of a J-shaped running blade for short-distance Paralympic sprinting (100–200 m), with comparative analysis between composite laminates and aluminium alloy.

📌 Project Goal

Develop the lightest blade configuration able to:

Withstand a 2000 N ground reaction load

Limit tip displacement to 40 mm (target stiffness ≈ 50 N/mm)

Satisfy failure criteria

The study combines analytical modelling, composite laminate theory, and finite element simulations.

🧠 Methodology
Geometry

3D CAD model (SolidWorks) inspired by the “Cheetah Xtreme” concept

Shell-based modelling approach

Analytical Model

2D beam simplification

Identification of the critical curved (“S-shaped”) region

Finite Element Analysis (Abaqus/CAE)

Static General step

2000 N applied as pressure at blade tip

Encastre constraint at socket interface

Tsai–Hill criterion for composites

Von Mises criterion for aluminium

Progressive ply optimization

🧵 Materials Investigated

CFRP (Carbon Fiber Reinforced Polymer)

GFRP (Glass Fiber Reinforced Polymer)

AA7075 Aluminium Alloy

Two symmetric laminate stacking sequences were compared (with and without 90° plies).

📊 Key Results
Structural Integrity
Material	Plies Required
CFRP	28
GFRP	44

Laminates without 90° plies showed better performance under bending.

Displacement Target (≤ 40 mm)
Material	Final Plies	Weight
CFRP	52	1.75 kg
GFRP	84	3.5 kg
AA7075	—	2.8 kg
🏆 Final Selection

CFRP provides the best stiffness-to-weight ratio and meets both failure and displacement constraints with the lowest mass.

Metallic solutions, although structurally viable, result in higher inertial mass and lower performance efficiency for sprint applications.

🏭 Manufacturing Assessment

Selected process: Prepreg Vacuum Bagging

Reasons:

Controlled fiber orientation

High repeatability

Industrial feasibility for customized prosthetics

🔧 Tools Used

SolidWorks (CAD)

Abaqus/CAE (FEA)

Classical Lamination Theory
