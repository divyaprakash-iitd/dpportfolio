---
title: "Geometry Generator Scripts: Learning Shell Scripting"
excerpt: "A collection of Bash scripts developed during my Masters for learning shell scripting, focusing on automated geometry generation for OpenFOAM cases using GMSH.<br/><img src='images/geometry-generator.png'>"
collection: portfolio
---

# Geometry Generator Scripts

## Project Overview
During my Masters studies, I developed these Bash scripts as a learning exercise to understand shell scripting while working with OpenFOAM cases. The project focuses on automating the generation of simple 3D geometries (boxes and cylinders) using GMSH, which could later be used in OpenFOAM simulations.

## Key Features
- **Interactive Geometry Creation**: Command-line interface for defining geometric parameters
- **Multiple Geometry Types**: Support for boxes and cylinders in 3D space
- **Batch Processing**: Ability to generate multiple geometries in sequence
- **GMSH Integration**: Automatic generation of GMSH (.geo) files
- **Learning Outcomes**: 
  - Basic shell scripting concepts
  - Command-line input handling
  - File manipulation in Bash
  - GMSH geometry file format
  - Process automation

## Technical Details
- **Implementation**: Bash shell scripts
- **Dependencies**: GMSH
- **Input**: Interactive command-line prompts
- **Output**: GMSH geometry files (.geo)

## Implementation Highlights
The project consists of three main scripts that work together to create geometric configurations. Here's a sample interaction:

```bash
$ ./run_all.sh
Enter Number of boxes: 
1
Enter Number of cylinders: 
1
Box Details
Enter P1 (x1 y1 z1): 0 0 0
Enter P2 (x2 y2 z2): 1 1 1
Cylinder Details: 
Enter P1 (x1 y1 z1): 0.5 0.5 0
Enter P2 (x2 y2 z2): 0.5 0.5 1
Enter Radius: 0.4
```

This creates a unit cube with a vertical cylinder passing through it - a common test case for OpenFOAM simulations. The scripts handle:

- Coordinate calculations for all geometry vertices
- GMSH format compatibility
- Automated file generation and visualization
- Interactive user input processing

## Repository Structure
```
.
├── run_all.sh
├── dp_script_box.sh
├── dp_script_cylinder.sh
└── README.md
```

## Technical Documentation
[GitHub Repository](https://github.com/divyaprakash-iitd/visgeom)
