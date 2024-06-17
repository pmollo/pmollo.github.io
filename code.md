---
layout: default
title: Code
---

# Programming

<hr>
## Math for biomedical modelling
### Computational Fluid Dynamics
* [**Navier-Stokes benchmark**](https://gitlab.com/piemollo/cfd/ns-validation);
FreeFem code to validate and benchmark an unsteady NS solver.
* [**Dropipe**](https://gitlab.com/piemollo/cfd/dropipe);
FreeFem code to validate pressure drop in CFD simulation.
* **Cerebral Venous Network**; [currently private] 
FreeFem, Python and Octave codes to pre-process raw data from medical acquisitions,
simulate the venous blood flow and post-process results. 
* **2D Bifurcation sandbox problem**; [currently private]
FreeFem and Octave of 2D vascular toy problem.
* [**Windkessel BC for FreeFEM**](https://gitlab.com/piemollo/cfd/windkessel-ff)
`.idp` file to build implicit Windkessel BC matrices in FreeFEM.

### Physiological modelling
* [**Flow rate manager**](https://gitlab.com/piemollo/phimod/frm);
Octave module to process and resample flow rate acquisition.
* **Center lines**; [currently private] 
Octave module to load, display and manage center line from vessel networks.

<hr>
## Reduced Order Modelling
### Reduced Basis Methods
* **Proper Orthogonal Decomposition**; 
[FreeFEM version](https://gitlab.com/piemollo/rom/rbm/pod), 
[Octave version](https://gitlab.com/piemollo/rom/rbm/podmatlib), 
[Python version](https://gitlab.com/piemollo/rom/rbm/podpy)
modules to run POD on data sets, with test certification.
* [**Reduced Basis Suite**](https://gitlab.com/piemollo/rom/rbm/rbs);
FreeFem code to manage RB items [WiP].
* [Old Reduced Basis Code](https://gitlab.com/piemollo/rom/rbm/old-rbm);
FreeFem code to run Reduced Basis Method problems [depreciated].

### Associated modules
* **Empirical Interpolation Method**;
[FreeFEM version](https://gitlab.com/piemollo/rom/eim/ffeim);
[Octave version](https://gitlab.com/piemollo/rom/eim/eim-oct).
code to perform EIM on data set. 
* **Parametrized-Background Data-Weak**; [currently private] 
Octave module to run PBDW state estimations.

<hr>
## Numerical Analysis
* [**Radial Basis Function**](https://gitlab.com/piemollo/numa/rbf);
Octave module to perform RBF interpolation with several kernel functions.
* **Non-Parametric Estimation**; [currently private].

<hr>
## Miscellaneous
* [**Extended Linear Algebra FreeFem**](https://gitlab.com/piemollo/tb/elaf); 
FreeFem code to perform standard LA operations between arrays and matrices.
* [**FF Matlib**](https://gitlab.com/piemollo/tb/ffmatlib);
FreeFem/Octave module to interface data structures.
(forked project, original [here](https://github.com/samplemaker/freefem_matlab_octave_plot)).
* [**FF Python**](https://gitlab.com/piemollo/tb/ffpy);
FreeFem/Python code to interface data structures [WiP].
* [**Statistical Display Matlab**](https://gitlab.com/piemollo/tb/statistical-display-matlab-octave);
Matlab(c) code to display distributed data over several categories.
* [**Grid Manager**](https://gitlab.com/piemollo/tb/gridmng); 
Octave/Matlab(c) codes to manage 2D grid in 3D environment. 
Useful step to provide _in silico_ MRI measurements.
* [**Python Package template**](https://gitlab.com/piemollo/tb/python-project-template)
handy template to build Python package.
