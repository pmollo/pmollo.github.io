---
layout: default
title: Code
---

### [Home](./index.md)

# Programming

<hr>

## Biomedical modeling

### Computational Fluid Dynamics
* [**Navier-Stokes benchmark**](https://gitlab.com/piemollo/cfd/ns-validation)
FreeFem code to validate and benchmark an unsteady NS solver.
* **Dropipe** FreeFem code to validate pressure drop in CFD simulation.
  * [2d version](https://gitlab.com/piemollo/cfd/dropipe-2d)
  * [3d version](https://gitlab.com/piemollo/cfd/dropipe-3d)
* [**Cerebral Venous Network**](https://zenodo.org/records/11032278)
FreeFem and Python codes to pre-process raw data from medical acquisitions,
simulate the venous blood flow and post-process results [2]. \
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11032278.svg)](https://doi.org/10.5281/zenodo.11032278).
* **2D Bifurcation sandbox problem**; [currently private]
FreeFem and Octave of 2D vascular toy problem.
* **Windkessel BC for FreeFEM**
`.idp` file to build implicit Windkessel BC matrices in FreeFEM [4].
  * [2d version](https://gitlab.com/piemollo/cfd/windkessel-ff-2d)
  * [3d version](https://gitlab.com/piemollo/cfd/windkessel-ff-3d)

### Physiological modeling
* [**Windkessel 0d**](https://gitlab.com/piemollo/phimod/windkessel) 
Standalone Python code to test different Windkessel configurations.
* [**Flow rate manager**](https://gitlab.com/piemollo/phimod/frm)
Octave module to process and resample flow rate acquisition.
* **Center lines**; [currently private] 
Octave module to load, display and manage center line from vessel networks.

### Diffusion based problems
* [**Eye ball model**](https://gitlab.com/piemollo/diffusion/eye-ball-model)
Standalone Python project to run heat diffusion simulation in human eye ball,
problem proposed and studied in [3].
* [**2d brain NIRS**](https://gitlab.com/piemollo/diffusion/brain-slice-model)
Standalone Python project to run light propagation simulation in real-life
brain 2d geometry,
problem proposed and studied in [1].
* [**Simplified NIRS**](https://gitlab.com/piemollo/diffusion/simplified-nirs)
Standalone Python project to run light propagation simulation in simplified
mutli-layer brain geometry,
problem proposed and studied in [5].

## Reduced Order Modeling

### Reduced Basis Methods
* **Proper Orthogonal Decomposition** modules to run POD on data sets, with test certification.
  * [FreeFEM version](https://gitlab.com/piemollo/rom/rbm/pod), 
  * [Octave version](https://gitlab.com/piemollo/rom/rbm/podmatlib), 
  * [Python version](https://gitlab.com/piemollo/rom/rbm/podpy)
* [**Reduced Basis Suite**](https://gitlab.com/piemollo/rom/rbm/rbs)
FreeFem code to manage RB items [WiP].
* [Old Reduced Basis Code](https://gitlab.com/piemollo/rom/rbm/old-rbm)
FreeFem code to run Reduced Basis Method problems [depreciated].

### Associated modules

* **Empirical Interpolation Method** code to perform EIM on data set. 
  * [Python version](https://gitlab.com/piemollo/rom/eim/eim-py).
  * [FreeFEM version](https://gitlab.com/piemollo/rom/eim/ffeim)
  * [Octave version](https://gitlab.com/piemollo/rom/eim/eim-oct).
* **Parametrized-Background Data-Weak** code to run PBDW state estimations [WiP].

## Data assimilation

### Linear state estimation
[WiP]

### Ensemble Methods
* **Ensemble Kalman Method** Method to solve parameter estimation problems
  * [Octave/Matlab(c) module](https://gitlab.com/piemollo/da/enkm/enkm-matlib) 
  * [Python] [WiP] 
* **Ensemble Kalman Filter** [WiP]

## Numerical Analysis
* [**Radial Basis Function**](https://gitlab.com/piemollo/numa/rbf);
Octave module to perform RBF interpolation with several kernel functions.
* **Non-Parametric Estimation** [WiP]

## Other numerical models
* [**2d Graetz problem**](https://gitlab.com/piemollo/diffusion/graetz-2d)
Standalone Python code to run 2d Graetz problem described in [7].
* [**Thermal bloc problem**](https://gitlab.com/piemollo/diffusion/thermal-single-block)
Standalone Python code to run thermal bloc problem described in [6].

## Miscellaneous

### [Freefem](https://freefem.org/) utils
* [**Extended Linear Algebra FreeFem**](https://gitlab.com/piemollo/tb/elaf)
FreeFem code to perform standard LA operations between arrays and matrices.
* [**FF Matlib**](https://gitlab.com/piemollo/tb/ffmatlib)
FreeFem/Octave module to interface data structures.
(forked project, original [here](https://github.com/samplemaker/freefem_matlab_octave_plot)).
* [**FF Python**](https://gitlab.com/piemollo/tb/ffpy)
FreeFem/Python code to interface data structures [WiP].

### Other
* [**Statistical Display Matlab**](https://gitlab.com/piemollo/tb/statistical-display-matlab-octave)
Matlab(c) code to display distributed data over several categories.
* [**Grid Manager**](https://gitlab.com/piemollo/tb/gridmng)
Octave/Matlab(c) codes to manage 2D grid in 3D environment. 
Useful step to provide _in silico_ MRI measurements.
* [**Python Package template**](https://gitlab.com/piemollo/tb/python-project-template)
handy template to build Python package.

<hr>

# References

[1] B. Sulis, “Analyse multimodale et problèmes inverses pour l’imagerie cérébrale.,” 
These de doctorat, Reims, 2024. 
Available: https://theses.fr/2024REIMS006 \
[2] P. Mollo, G. Dollé, S. Salmon, and O. Balédent, “Accurate Cerebral Venous Blood Flow Simulations Compared to Real Data,” Apr. 2024. doi: 10.5281/zenodo.11032278. \
[3] T. Saigre, C. Prud’homme, and M. Szopos, “Model order reduction and sensitivity analysis for
complex heat transfer simulations inside the human eyeball”, 
International Journal for Numerical Methods in Biomedical Engineering, vol. 40, no. 11, p. e3864, 
2024, doi: 10.1002/cnm.3864. \
[4] P. Mollo, “Coupling 2D/3D fluid models with 0D Windkessel model via boundary condition,” Oct. 2023. Available: https://hal.science/hal-04247891 \
[5] F. Oumri, “Modélisation mathématique, simulation numérique et application en tomographie optique 
chez l’enfant prématuré,” 
These de doctorat, Reims, 2021. 
Available: https://www.theses.fr/2021REIMS003 \
[6] N. Aretz-Nellesen, M. A. Grepl, and K. Veroy, “3D-VAR for Parametrized Partial Differential 
Equations: A Certified Reduced Basis Approach,” 
May 14, 2019, arXiv: arXiv:1905.05817. doi: 10.48550/arXiv.1905.05817. \
[7] J. S. Hesthaven, G. Rozza, and B. Stamm, Certified Reduced Basis Methods for Parametrized Partial 
Differential Equations. in SpringerBriefs in Mathematics. 
Cham: Springer International Publishing, 2016. doi: 10.1007/978-3-319-22470-1.


<hr>

# More

### [home](./index.md)
### [Communications](./presentations.md)
### [Teaching activity](./teaching.md)
### Galery

<hr>