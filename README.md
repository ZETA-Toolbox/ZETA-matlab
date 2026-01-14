# ZETA

**Z**onotope-based **E**s**T**imation and f**A**ult diagnosis of discrete-time systems

- Check our [paper](https://doi.org/10.1109/CDC57313.2025.11312660) presented at the 64th IEEE Conference on Decision and Control (or the [preprint](https://arxiv.org/abs/2504.06467))
- by Brenner S. Rego, Joseph K. Scott, Davide M. Raimondo, Marco H. Terra and Guilherme V. Raffo

ZETA is a MATLAB library featuring implementations of set representations based on zonotopes, namely: 
- [Zonotopes](https://doi.org/10.1007/BF02684450),
- [Constrained zonotopes](https://web.mit.edu/braatzgroup/Scott_Automatica_2016.pdf), and
- [Line zonotopes](https://doi.org/10.1016/j.automatica.2025.112380),
  
in addition to a basic implementation of [interval arithmetic](https://en.wikipedia.org/wiki/Interval_arithmetic). 

This library has capabilities starting from the basic set operations with
these sets, including propagations through nonlinear functions using
various approximation methods. The features of ZETA allow for
reachability analysis and state estimation of discrete-time linear,
nonlinear, and descriptor systems, in addition to active fault diagnosis
of linear systems. Efficient order reduction methods are
also implemented for the respective set representations. 

- This library requires [YALMIP](https://yalmip.github.io/) to work properly.

- ZETA supports [GUROBI](https://www.gurobi.com/) for efficient solutions of the underlying optimization problems.

- [MPT](https://www.mpt3.org/) is required in a few demonstration examples, while allowing for extended plotting capabilities.

The library is initialized by running `zeta_init.m`.

### Citation

If you have used this library as part of your work, cite it as follows:
```
@inproceedings{Rego2025ZETA,
author={Rego, Brenner S. and Scott, Joseph K. and Raimondo, Davide M. and Terra, Marco H. and Raffo, Guilherme V.},
booktitle={2025 IEEE 64th Conference on Decision and Control (CDC)}, 
title={ZETA: a library for Zonotope-based EsTimation and fAult diagnosis of discrete-time systems}, 
year={2025},
pages={2420--2427}
}
```
