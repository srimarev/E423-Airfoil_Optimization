# E423-Airfoil_Optimization
# Airfoil Shape Optimization using Eppler 423 (E423)

## Overview

This project focuses on the optimization of the Eppler 423 (E423) airfoil to improve aerodynamic efficiency under specified operating conditions.

## Objective

Improve the Lift-to-Drag Ratio (L/D) while satisfying:

- Reynolds Number = 500,000
- Mach Number = 0.1
- Angle of Attack = 5°
- Minimum thickness-to-chord ratio ≥ 10%

## Methodology

1. Airfoil screening using UIUC database
2. Baseline selection (E423)
3. Parametric geometry optimization
4. XFLR5 aerodynamic analysis
5. ANSYS Fluent CFD validation

## Geometry Changes

| Parameter              | Baseline | Optimized |
|------------            |----------|-----------|
| Thickness (%)          | 12.52    | 10.03     |
| Thickness Position (%) | 26.13    | 23.72     |
| Max Camber (%)         | 10.05    | 10.50     |
| Camber Position (%)    | 44.04    | 44.04     |

## Results

| Parameter | Baseline | Optimized |
|-----------|----------|-----------|
| Cl @ 5°   | 1.590    | 1.676     |
| Cd @ 5°   | 0.01317  | 0.01289   |
| L/D @ 5°  | 120.743  | 129.944   |

### Improvement

L/D Improvement = 7.62%

### CFD Validation

Baseline Cl = 0.47

Optimized Cl = 0.50

Lift Improvement = 6.4%

## Tools Used

- XFLR5
- ANSYS Fluent
- SolidWorks

## Team Members

- Srima Santosh Revankar
- Rishit Kumar
- Shreyas Deshmukh
- Sai Arvind Akella
