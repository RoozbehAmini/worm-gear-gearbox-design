# worm-gear-gearbox-design
Evaluation different designs for a cooling tower transmission - Full Design and Optimization of a Worm-Gear Gearbox
# Cooling Tower Fan Transmission - Worm Gear Gearbox Design

## Overview
This repository contains the complete mechanical design, mathematical optimization, and CAD models for an industrial cooling tower fan drive transmission system. The objective of this project is to transfer mechanical power from a 55 kW horizontal electric motor to a vertical 4-metre-diameter axial-flow fan blade. 

After a rigorous comparative analysis against a bevel-helical alternative, a **single-stage worm gear configuration** was selected and optimized to meet the strict spatial and weight constraints of the cooling tower's elevated mounting frame.

This project was completed for the Machine Elements Design course at the University of Tehran, supervised by Dr. Masoud Shariat Panahi.

## System Requirements
*   **Fan Blade Diameter:** 4 meters
*   **Air Exit Velocity:** 12 m/s
*   **Volumetric Flow Rate:** ~150.8 m³/s
*   **Required Fan Speed:** 110 rpm
*   **Input Motor:** 55 kW (IEC 225M Frame), 1475 rpm
*   **Reduction Ratio:** 13.41:1

## Design Optimization
A custom MATLAB optimization algorithm was developed to determine the Pareto-optimal geometry for the worm gear set. The algorithm swept through axial pitches from 40mm to 70mm, calculating the minimum feasible worm diameter (satisfying AGMA safety factors ≥ 1.5) and conducting a pairwise tournament scoring system based on:
1.  **Gearbox Mass** (Minimized)
2.  **Bounding Volume** (Minimized)
3.  **Mesh Efficiency** (Maximized)

The winning design utilizes a **52 mm axial pitch**, achieving an optimal balance with an estimated internal mass of 234 kg and a mesh efficiency of 88.34%.

## Final Technical Specifications
| Component | Description | Key Dimensions / Details |
| :--- | :--- | :--- |
| **Worm Gear Pair** | $p = 52$ mm, $N_w = 3$, $N_G = 41$ | $d_w = 93.2$ mm, $d_G = 678.6$ mm |
| **Worm Shaft** | AISI 4140 Q&T, stepped | 28 - 54 mm range |
| **Gear Shaft** | AISI 4140 Q&T, stepped | 55 - 80 mm range |
| **Worm Bearings** | SKF 32207 + SKF 31309 (Tapered) | Rated life: 72,500 h |
| **Gear Bearings** | SKF 7311 BECBY (x2) | 55 mm bore |
| **Seals** | SKF HMSA10RG Lip Seal | 40 x 55 x 7 mm |
| **Input Coupling** | Rotex 160 | 877 N-m rated |
| **Output Coupling**| Rexnord Omega 425 | 5580 N-m rated |


