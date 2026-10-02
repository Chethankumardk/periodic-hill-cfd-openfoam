# Project Documentation

## Project Context

This repository presents a Computational Fluid Dynamics study of three-dimensional, steady-state, incompressible turbulent flow over a periodic hill using OpenFOAM.

The periodic-hill configuration was used to investigate numerical convergence, mesh sensitivity, discretization schemes, solver parameters, and flow-field characteristics.

## Project Type

This work was completed as a university team project.

The original academic report identifies three project members. This public repository focuses on the technical CFD methodology and results and intentionally excludes student identification numbers and other administrative information.

Individual contributions are not separately documented in the retained project evidence.

## Tools and Methods

The documented workflow includes:

- OpenFOAM
- ParaView
- RANS simulation
- Structured hexahedral meshing with `blockMesh`
- Grid-independence analysis
- Residual convergence monitoring
- Velocity-profile analysis
- Vorticity visualization
- Q-criterion visualization
- Numerical-scheme comparison
- Solver-parameter sensitivity studies

The project report also states that plotting was performed using Python. However, the original plotting scripts are not included in this repository because retained source code for those plots is not available.

## Grid Independence Study

Four mesh resolutions were investigated:

- Grid 1: 5,000 cells
- Grid 2: 40,000 cells
- Grid 3: 320,000 cells
- Grid 4: 2,560,000 cells

The study found close agreement between Grid 3 and Grid 4 velocity profiles. Grid 3 was therefore selected for subsequent analysis as a balance between numerical resolution and computational cost.

## Numerical Analysis

The study investigated the effects of:

- Mesh refinement
- First-order and second-order discretization schemes
- Linear-solver tolerances
- Relaxation factors
- Non-orthogonal correctors
- Residual-control settings

Post-processing was used to examine velocity profiles, vorticity, Q-criterion structures, and convergence behavior.

## Repository Scope

This repository contains a retained OpenFOAM case configuration together with selected numerical results and visualizations.

Large generated OpenFOAM result directories, decomposed processor directories, redundant intermediate files, and the original academic report are intentionally excluded.

The original report is not published here because it contains student identification information and academic administrative material.

## Evidence and Reproducibility Note

The `case/` directory contains retained OpenFOAM configuration files associated with the project.

Because multiple numerical configurations were investigated during the study, the retained case should not be interpreted as a complete archive of every grid, discretization scheme, tolerance case, or relaxation-factor configuration discussed in the report.
