---
title: "libaxb: High-Performance Linear System Solver"
excerpt: "A C++/Fortran library for solving sparse linear systems using BiCGSTAB with ILU preconditioning, featuring OpenMP parallelization and a robust CRS format matrix input system.<br/><img src='/images/libaxb-diagram.png'>"
collection: portfolio
---

# libaxb: Sparse Linear System Solver

## Project Overview
`libaxb` is a high-performance numerical library designed to solve sparse linear systems of equations (Ax=b). Built with C++ and offering both C++ and Fortran interfaces, it combines the efficiency of the Eigen template library with OpenMP parallelization to provide a robust solution for large-scale scientific computing problems.

## Key Features
- **Efficient Matrix Storage**: Uses Compressed Row Storage (CRS) format for optimal memory usage
- **Advanced Solver**: Implements BiCGSTAB (Bi-Conjugate Gradient Stabilized) method with ILU (Incomplete LU) preconditioning
- **Cross-Language Support**: Seamlessly integrates with both C++ and Fortran applications
- **Performance Optimized**: Leverages OpenMP parallelization and high-level optimization flags
- **Memory Efficient**: Global matrix storage enables multiple solves with different right-hand sides

## Technical Details
- **Implementation**: C++ with Fortran interface via ISO_C_BINDING
- **Dependencies**: Eigen3, OpenMP
- **Build System**: CMake
- **Input Format**: Text-based CRS format input system
- **Solver Parameters**:
  - BiCGSTAB tolerance: 1e-6
  - Maximum iterations: 1000
  - ILU preconditioner drop tolerance: 1e-4

## Target Applications
- Finite Element Analysis
- Computational Fluid Dynamics
- Structural Engineering
- Circuit Analysis
- Any scientific computing application requiring sparse linear system solutions

## Implementation Highlights
```cpp
// C++ Interface
SparseSolver::initialize(values, col_indices, row_ptrs, rows, cols, nnz);
SparseSolver::solve(rhs, rhs_size, solution);
```

```fortran
! Fortran Interface
call initialize_sparse_matrix(values, col_indices, row_ptrs, rows, cols, nnz)
call solve_sparse_system(rhs, rhs_size, solution, 1.0d-6, 1000)
```

## Repository Structure
The library is organized with a clean, modular structure:
- Core solver implementation in C++
- Fortran interface module
- Example implementations in both languages
- CMake build system for easy integration

## Technical Documentation
[GitHub Repository](https://github.com/divyaprakash-iitd/libaxb)
