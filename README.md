This code was written as part of a summer project that the author did with Prof. Nirmal Raj, Center for High Energy Physics, Indian Institute of Science.

# BBN-Abundance-Calculation
A basic BBN reaction network up to the $^7\text{Be}$ nuclide is considered to calculate the mass fraction of nuclides vs temperature (MeV) curve for a given vacuum expectation value (the weak scale). For this purpose, the reaction rates as given in the JINA Reaclib database were used. The code also outputs a reaction rate vs temperature curve for all the reactions involved.

The code produces the correct plots for the weak scale values between 50 GeV < v < 600 GeV. The lower bound is because the freeze out temperature begins to equalize with the bottleneck temperature, whereas the upper bound arises because of the temperature range in which the Reaclib reaction rates are valid.

The code also computes a bonus plot: $\text{Y}_4$ (this is the symbol used in BBN literature to denote the mass fraction of $^4\text{He}$) versus the weak scale.

#### References
[BBN-simple: How to Bake a Universe-Sized Cake](https://www.sciencedirect.com/science/article/pii/S1387647325000016?via%3Dihub) \
[The Weak Scale from BBN](https://arxiv.org/abs/1409.0551) 


### Example Plots
<img width="1020" height="527" alt="image" src="https://github.com/user-attachments/assets/fe0b9059-966e-46f8-9e67-8dd9b023a2d0" />   

<img width="856" height="591" alt="image" src="https://github.com/user-attachments/assets/6727bed8-3382-4ca2-9706-54a0f38342a7" />

<img width="711" height="529" alt="image" src="https://github.com/user-attachments/assets/266e169a-ad43-4c0d-adfd-d284652cd7d2" />



## Usage Section
Run the following commands in your terminal: \
git clone https://github.com/NottingTheNot/BBN-Abundance-Calculation \
pip install -r requirements.txt \
jupyter notebook plotting.ipynb

### Usage of AI in the code
Most the code as well as the entirety of the physics was decided by the author. However, some of the code pertaining to the stiff ODE solver;
wrapping part of the code with tqdm expressions to represent a progress bar; overcoming overflow errors in certain expressions; and making the plots look prettier were done with the help of AI. 

