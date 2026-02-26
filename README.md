# Sprint Running Blade Design  
Finite Element Optimization of Composite and Aluminium Solutions

## Overview

This project concerns the design and structural optimization of a J-shaped running blade intended for short-distance Paralympic sprinting (100–200 m).

The main goal was to identify the lightest configuration able to:

- Withstand a 2000 N ground reaction load  
- Limit the tip displacement to 40 mm (target stiffness ≈ 50 N/mm)  
- Satisfy appropriate structural failure criteria  

The work combines analytical modelling, Classical Lamination Theory and finite element simulations in Abaqus.

---

## Design Approach

### Geometry

The blade geometry was developed in SolidWorks, starting from literature dimensions and existing sprint blade concepts.  
The profile was modelled as a J-shaped structure and then implemented in Abaqus using a shell-based approach.

### Analytical Model

Before moving to FEA, a simplified 2D beam model was developed to:

- Estimate the bending moment distribution  
- Identify the most critical region  

Both analytical and numerical results indicate that the curved “S-shaped” region governs the structural behaviour.

### Finite Element Model (Abaqus/CAE)

A static general analysis was performed with:

- 2000 N applied as pressure on the blade tip  
- Encastre constraint at the socket interface  
- Mesh refinement in the curved region  

Failure criteria adopted:

- Tsai–Hill for composite laminates  
- Von Mises for aluminium  

Laminate thickness was progressively increased until both failure and displacement requirements were satisfied.

---

## Materials Investigated

- CFRP (Carbon Fiber Reinforced Polymer)  
- GFRP (Glass Fiber Reinforced Polymer)  
- AA7075 Aluminium Alloy  

Two symmetric laminate stacking sequences were compared to evaluate the influence of 90° plies under dominant bending loading.

---

## Results

### Structural Integrity (2000 N)

| Material | Plies Required to Avoid Failure |
|----------|--------------------------------|
| CFRP     | 28 |
| GFRP     | 44 |

Laminates without 90° plies showed better performance, requiring fewer layers to satisfy the Tsai–Hill criterion.

---

### Displacement Constraint (≤ 40 mm)

| Material | Final Configuration | Weight |
|----------|-------------------|--------|
| CFRP     | 52 plies | 1.75 kg |
| GFRP     | 84 plies | 3.5 kg |
| AA7075   | 1.2 cm thickness | 2.8 kg |

CFRP achieves the displacement target with the lowest mass.

---

## Final Considerations

CFRP provides the best stiffness-to-weight ratio among the investigated materials and satisfies both strength and displacement constraints with the lowest inertial mass.

Although AA7075 meets the displacement requirement, its higher density makes it less competitive for sprint-specific applications.  
GFRP, while cheaper, requires a significantly higher thickness and results in excessive weight.

---

## Manufacturing Assessment

Among the manufacturing processes reviewed, prepreg vacuum bagging was identified as the most suitable solution due to:

- Better control of fiber orientation  
- Improved repeatability  
- Higher mechanical consistency compared to hand lay-up  

---

## Tools and Methods

- SolidWorks – CAD modelling  
- Abaqus/CAE – Finite Element Analysis  
- Classical Lamination Theory  
- Composite failure modelling (Tsai–Hill)

---

## Key Takeaways

- The curved region controls stress concentration and structural performance.  
- 90° plies are detrimental under the considered loading condition.  
- Weight reduction is the dominant parameter in sprint blade design.  
- CFRP is clearly the most efficient material for this application.
