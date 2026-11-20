<img width="2590" height="2275" alt="2D_ODW_Contours" src="https://github.com/user-attachments/assets/907afefc-cfd9-4b30-928b-14b23fe655de" />
<img width="3300" height="1926" alt="2D_ODW_Visualization" src="https://github.com/user-attachments/assets/6ea99931-70e0-4a28-bf05-90dc39692c1b" />
# oblique-detonation-wave-detonationFoam
# Oblique Detonation over a Wedge (`detonationFoam`)

This repository contains the preliminary/initial case setup for simulating an **Oblique Detonation Wave (ODW)** over a wedge geometry using **detonationFOAM** in **OpenFOAM-v8**. The case incorporates detailed chemical kinetics based on the **Burke et al. mechanism**.

## Technical Specifications
* **Solver:** detonationFOAM
* **OpenFOAM Version:** OpenFOAM-v8
* **Configuration:** 2D/3D Oblique Detonation over a Wedge
* **Chemical Mechanism:** Burke et al. reaction mechanism
* **Current Status:** Initial Setup / Preliminary Grid and Boundary Condition Verification

## Objectives & Focus Areas
* Investigating the initiation and stabilization of oblique detonation waves behind an induced wedge shock.
* Analyzing the coupling between the oblique shock wave and the reactive combustion zone (induction length, reaction zone structure).
* Validating initial thermodynamic and transport properties using the Burke et al. kinetic model.

## Preliminary Case Structure
* `0/` - Initial boundary conditions for wedge flow (velocity, pressure, temperature, and species mass fractions).
* `constant/` - Transport properties, thermodynamic databases, and the **Burke et al.** chemical kinetics files (`chemistryProperties`, `reactions`, `thermo.compressibleGas`).
* `system/` - Mesh configuration (`blockMeshDict` / snappyHexMesh), control dictionary (`controlDict`), and numerical discretization schemes (`fvSchemes`, `fvSolution`).

## Prerequisites
* **OpenFOAM-v8** compiled with `detonationFOAM`.

## Future Work / Next Steps
* Refine the mesh near the wedge leading edge to capture the sharp induction zone.
* Perform grid convergence studies on oblique shock angles.
