Fast solvers for two-dimensional scattering problems in 2D are presented.

By representing the scattered field as a volume potential in terms of the Green's function, we arrive at the Lippmann-Schwinger equation in integral form.

This repository has 4 projects to solve the Lippmann-Schwinger equation via volume integral equation using 3 techniques.

1. HODLR: HODLR based direct solver.

2. GMRES: GMRES based iterative solver. The matrix-vector products encountered in each of its iteration have been computed using DAFMM (Directional Algebraic Fast Multipole Method). All the low rank factorisations encountered were formed using Nested Cross Approximation (NCA).

3. Hybrid: GMRES based iterative solver with HODLR as pre-conditioner.

4. GMRES_Hybrid: This is a new version of the code, where both GMRES and Hybrid solvers can be run from the same file. This also uses a different variant of GMRES routine.

For more details please refer article [[1](https://doi.org/10.4208/cicp.OA-2022-0103)](#1).

The inputs to the codes are to be given at run-time, the details of which have been given in the Readme.md files of the respective projects.

The value of Phi and the real part of the field get stored in a directory called result, which gets created at run-time.

## References
<a id="1">[1]</a>
Ambikasaran, S., Gujjula, V. (2022). A New Directional Algebraic Fast Multipole Method Based Iterative Solver for the Lippmann-Schwinger Equation Accelerated with HODLR Preconditioner. Communications in Computational Physics, 32(4), 1061-1093.
