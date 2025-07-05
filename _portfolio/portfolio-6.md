---
title: "FEM Simulation of Large Deformations in 2D and 3D Structures"
excerpt: "A MATLAB and Fortran-based Finite Element Method (FEM) library for simulating large deformations in 2D and 3D geometries. <br/><img src='/images/ellipsoidal_shell.gif'>"
collection: portfolio
---

## Overview
Developed a modular FEM simulation library in MATLAB and Fortran to model large deformations in soft 2D and 3D materials. The framework, demonstrated on annular and volumetric domains, supports mesh generation via Gmsh and leverages hyperelastic material models to simulate deformation under applied forces.

## Technical Highlights
- Implements FEM using triangular (2D) and tetrahedral (3D) elements with explicit time integration
- Calculates internal forces based on deformation tensors and hyperelastic models
- Supports arbitrary 2D and 3D meshes with physical groups defined in Gmsh
- Modular code architecture: separate routines for shape function coefficients, cofactor matrix computation, and force assembly
- Boundary identification and force application via physical group tagging
- Extended functionality with Fortran for enhanced computational efficiency in 3D simulations

## Impact
The library enables rapid prototyping and investigation of material deformation under various boundary conditions in both 2D and 3D. Its flexible design supports research in soft matter physics, material science, and bioengineering simulations.

## Skills Demonstrated
- Finite Element Method
- Hyperelastic Material Modeling
- Scientific Computing with MATLAB and Fortran
- Mesh Generation with Gmsh
- Deformation Visualization
- 3D Simulation Development

## Technical Documentation
[GitHub Repository](https://github.com/divyaprakash-iitd/flexFEM)

---

