---
title: "FEM Simulation of Large Deformations in 2D Structures"
excerpt: "A MATLAB-based Finite Element Method (FEM) library for simulating large deformations in 2D geometries, demonstrated on an annular (donut-shaped) mesh.<br/><img src='/images/cfd_gallery/donut_animation.webp'>"
collection: portfolio
---

## Overview
Developed a modular FEM simulation library in MATLAB to model large deformations in soft 2D materials. The framework, demonstrated on an annular domain, supports mesh generation via Gmsh and leverages hyperelastic material models to simulate deformation under applied forces.

## Technical Highlights
- Implements FEM using triangular elements and explicit time integration
- Calculates internal forces based on deformation tensors and hyperelastic models
- Supports arbitrary 2D meshes with physical groups defined in Gmsh
- Modular code architecture: separate routines for shape function coefficients, cofactor matrix computation, and force assembly
- Boundary identification and force application via physical group tagging

## Impact
The library enables rapid prototyping and investigation of material deformation under various boundary conditions. Its flexible design supports research in soft matter physics, material science, and bioengineering simulations.

## Skills Demonstrated
- Finite Element Method
- Hyperelastic Material Modeling
- Scientific Computing with MATLAB
- Mesh Generation with Gmsh
- Deformation Visualization

## Technical Documentation
[GitHub Repository](https://github.com/divyaprakash-iitd/flexFEM)

