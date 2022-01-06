# Landscape Evolution Model (LEM) Stability Analysis
- This is a Python code to numerically compute the solution of the linear stability analysis problem for the detachment-limited landscape evolution model (LEM).
- Using the developed code, the role of _m_ and _n_ (exponents of the specific drainage area and slope, respectively in the fluvial erosion term of the model) on the onset and selection of regular valley spacing can be examined.

# Publication
The submitted research work can be found here: .
# Installation
- Required python libraries are numpy and scipy libraries. 

- This repository contains the code as a jupyter notebook, which can be installed using using pip as `pip install notebook` or using Conda `conda install -c conda-forge notebook`.

- Files **s200.mat** and **w200.mat** in the repository contain 200 Quadrature Points and Weight Functions, respectively, for the numerical solver.

# Code structure
Each number written in the list below explains the operations and functions for the particular Cell of the Jupyter Notebook.
1. Import relevant packages from  numpy and scipy libraries.
2. Import quadrature points and weight functions arrays (**s200.mat** and **w200.mat**), define Python functions for trial and test functions used in the weak formulation, and define Python functions to numerically obtain the slope and its derivatives for generic values of _m_ and _n_.
3. Select values of parameters (_C<sub>I</sub>,m,n,L,U,k_), global variables and arrays used in the solver.
4. For every Channelization Index (_C<sub>I</sub>_) and wavenumber (_k_), solve the eigen-value problem using spectral Galerkin technique with numerical quadrature.
5. Extract the critical Channelization Index _C<sub>I<sub>cr</sub></sub>_  and the corresponding fastest growing (positive) spatial frequency (_k<sub>cr</sub>_).
6. Save relevant arrays for plotting and further investigations.

# Contact Us
For more information about this research, you can reach out to us at [Shashank Kumar Anand](mailto:skanannd@princeton.edu?subject=[GitHub]%20Landscape%20Evolution%20Model%20(LEM)%20Stability%20Analysis) or [Amilcare Porporato](mailto:aporpora@princeton.edu?subject=[GitHub]%20Landscape%20Evolution%20Model%20(LEM)%20Stability%20Analysis). 

# Other Relevant Links
Well-commented Python code for the numerical simulations of the Landscape Evolution Model (LEM) by the same author is available at [github.com/ShashankAnand1996/LEM](https://github.com/ShashankAnand1996/LEM). The developed code here has been tested to provide efficient and accurate solutions of the LEM in detachment-limited conditions. The published manuscript is also available at [Linear layout of multiple flow-direction networks for landscape-evolution simulations](https://doi.org/10.1016/j.envsoft.2020.104804).
