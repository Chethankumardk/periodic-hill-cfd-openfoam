# OpenFOAM System Configuration

This directory contains the numerical and run-control configuration for the periodic-hill OpenFOAM case.

Included files:

- `blockMeshDict` — structured mesh definition and periodic-hill geometry
- `controlDict` — simulation control and residual monitoring
- `fvSchemes` — discretization schemes
- `fvSolution` — linear solvers, SIMPLE settings, convergence criteria, and relaxation factors
- `fvOptions` — mean-velocity forcing
- `decomposeParDict` — domain decomposition settings for parallel computation
- `topoSetDict` — cell/face set and zone definitions
