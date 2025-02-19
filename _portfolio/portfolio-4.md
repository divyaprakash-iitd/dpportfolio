---
title: "A Boundary Element Method (BEM) Solver"
excerpt: "Solves the 2D Laplace equation on a circular surface using using the Boundary Integral Method.<br/><img src='/images/bem.png'>"
collection: portfolio
---

## Project Overview

The **Boundary Element Method (BEM) Solver** is a MATLAB-based tool designed to solve the 2D Laplace equation over a circular domain. This solver employs the Boundary Integral Method, applying Dirichlet boundary conditions on one half of the boundary and Neumann boundary conditions on the other. The implementation is grounded in the methodologies presented in *A Beginner's Course in Boundary Element Methods* by Why-Teong Ang.

## Key Features

- **Boundary Integral Approach**: Utilizes the BEM to transform the domain problem into a boundary problem, reducing dimensionality and computational effort.
- **Flexible Boundary Conditions**: Supports both Dirichlet (fixed value) and Neumann (flux) boundary conditions, offering versatility in problem-solving.
- **Efficient Computation**: Employs numerical integration and linear system solvers to handle the integral equations efficiently.
- **Visualization Tools**: Includes functions to visualize the solution over the domain, aiding in analysis and interpretation.

## Technical Details

- **Language**: MATLAB
- **Core Functions**:
  - `bem_model.m`: Initializes the boundary element model.
  - `apply_boundary_conditions.m`: Assigns Dirichlet and Neumann conditions.
  - `construct_axb.m`: Constructs the system of linear equations.
  - `solver.m`: Solves the linear system to find boundary values.
  - `calculate_domain.m`: Evaluates the solution within the domain.
  - `plot_solution.m`: Visualizes the computed solution.
- **Dependencies**: Requires MATLAB R2022a or later.

## Implementation Highlights

The solver discretizes the boundary into elements, applies the specified boundary conditions, and constructs a system of linear equations representing the problem. By solving this system, it determines the unknown boundary values, which are then used to compute the solution at any point within the domain. Visualization functions are provided to plot the potential field, offering insights into the solution's behavior.

## Technical Documentation
[GitHub Repository](https://github.com/divyaprakash-iitd/bem.git)



