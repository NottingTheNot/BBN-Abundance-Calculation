# BBN-Abundance-Calculation
A basic BBN reaction network up to the $^7\text{Be}$ nuclide is considered to calculate the mass fraction of nuclides vs temperature (MeV) curve for a given vacuum expectation value (the weak scale). For this purpose, the reaction rates as given in the JINA Reaclib database were used. The code also outputs a reaction rate vs temperature curve for all the reactions involved.

The code produces the correct plots for the weak scale values between 50 GeV < v < 600 GeV. The lower bound is because the freeze out temperature begins to equalize with the bottleneck temperature, whereas the upper bound arises because of the temperature range in which the Reaclib reaction rates are valid.

The code also computes a bonus plot: $\text{Y}_4$ (this is the symbol used in BBN literature to denote the mass fraction of $^4\text{He}$) versus weak scale.
### Usage of AI in the code
Most the code as well as the entirety of the physics was decided by the author. However, there were still a few places in which AI was used. Specifically, some of the code pertaining to the stiff ODE solver;
wrapping part of the code with tqdm expressions to represent a progress bar; overcoming overflow errors in certain expressions; and making the plots look prettier are the places in which AI has been used.  

