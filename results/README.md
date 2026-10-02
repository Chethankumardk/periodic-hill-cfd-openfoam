# Numerical Study Results

This directory summarizes the main numerical findings from the periodic-hill CFD study.

## Grid Independence

Four structured meshes were investigated:

| Grid | Number of Cells |
|---|---:|
| Grid 1 | 5,000 |
| Grid 2 | 40,000 |
| Grid 3 | 320,000 |
| Grid 4 | 2,560,000 |

The coarse grids showed stronger mesh sensitivity, while the velocity profiles obtained with Grid 3 and Grid 4 were very similar.

Grid 3 was selected for the remaining analysis because it provided a practical balance between solution accuracy and computational cost.

## Numerical Schemes

First-order upwind and second-order linear discretization schemes were compared.

The first-order scheme showed smoother convergence but greater numerical diffusion.

The second-order scheme captured sharper velocity gradients and was preferred in the study for detailed flow analysis.

## Flow-Field Analysis

The CFD results were post-processed to examine:

- Streamwise and wall-normal velocity profiles
- Flow separation and recovery
- Vorticity distribution
- Q-criterion vortex structures
- Residual convergence

## Solver Sensitivity

The study also investigated the influence of:

- Linear-solver tolerances
- Relaxation factors
- Non-orthogonal correctors
- Residual-control settings

These comparisons were used to evaluate numerical stability, convergence behavior, and computational efficiency.

## Repository Scope

Large OpenFOAM time directories, decomposed processor directories, and redundant simulation outputs are intentionally excluded from this repository.

Selected plots and flow visualizations are available in the `images/` directory.
