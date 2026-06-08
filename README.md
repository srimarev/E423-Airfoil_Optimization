# E423-Airfoil_Optimization
# Airfoil Shape Optimization using Eppler 423 (E423)

## Overview

This project focuses on the aerodynamic optimization of the Eppler 423 (E423) airfoil to improve lift-to-drag ratio (L/D) under the specified operating conditions of the Honeywell Aerospace Design-A-Thon challenge.

## Problem Statement
Optimize an airfoil from the UIUC Airfoil Database to achieve maximum aerodynamic efficiency while satisfying the following constraints:

- Reynolds Number: 500,000
- Mach Number: 0.1
- Angle of Attack: 0°–10°
- Minimum thickness-to-chord ratio: 10%

## Methodology

1. Screened multiple UIUC airfoils using XFLR5.
2. Selected E423 as the baseline airfoil based on aerodynamic performance.
3. Performed constraint-driven geometric optimization by modifying:
   - Thickness-to-chord ratio
   - Maximum thickness position
   - Camber magnitude
4. Preserved structural feasibility by maintaining t/c ≥ 10%.
5. Evaluated aerodynamic performance using XFLR5.
6. Validated the optimized design through 3D CFD analysis in ANSYS Fluent.

## Airfoil Geometry Comparison

| Parameter              | Baseline | Optimized |
|------------------------|----------|-----------|
| Thickness (%)          | 12.52    | 10.03     |
| Thickness Position (%) | 26.13    | 23.72     |
| Max Camber (%)         | 10.05    | 10.50     |
| Camber Position (%)    | 44.04    | 44.04     |

## XFLR5 Results

| Parameter | Baseline | Optimized |
|-----------|----------|-----------|
| Cl @ 5°   | 1.590    | 1.676     |
| Cd @ 5°   | 0.01317  | 0.01289   |
| L/D @ 5°  | 120.743  | 129.944   |

### Performance Improvement

- Lift coefficient increased by approximately 5.4%
- Drag coefficient reduced
- Lift-to-drag ratio improved by approximately 7.6%

## CFD Validation

To complement the 2D XFLR5 analysis, a 3D CFD study was performed in ANSYS Fluent to account for finite-span effects and more realistic flow behavior.

### CFD Results

| Parameter             | Baseline E423 | Optimized E423 |
|-----------------------|---------------|----------------|
| Lift Coefficient (Cl) | 0.47          | 0.50           |

**Lift Improvement:** 6.4%

Velocity and pressure contours indicated stronger flow acceleration and a larger low-pressure region over the upper surface of the optimized airfoil, supporting the observed lift improvement.

## Tools Used

- XFLR5
- ANSYS Fluent
- SolidWorks

## Repository Contents

- Baseline E423 airfoil coordinates (.dat)
- Optimized E423 airfoil coordinates (.dat)
- XFLR5 aerodynamic analysis plots
- CFD velocity contours
- CFD pressure contours
- Final project presentation

## Team Members

- Srima Santosh Revankar
- Rishit Kumar
- Shreyas Deshmukh
- Sai Arvind Akella
