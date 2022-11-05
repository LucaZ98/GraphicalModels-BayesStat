# GraphicalModels-BayesStat
Project for the course Bayesian Statistics at Politecnico di Milano.

## Main goal
The aim of this project is to develop Bayesian methods for the analysis of multivariate categorical data. In particular, we are interested in inferring dependence relations between categorical variables, also accounting for possible heterogeneity related to latent clustering structures in the data.

## Personal contribution
We consider mixtures of graphical models to account for possible heterogeneous dependence relations among subjects, which can be linked to a latent clustering structure of the data. We base our model formulation on a Dirichlet Process (DP) mixture of graphical models.
With this representation it is possible to implement a MCMC scheme where parameters are integrated out and the algorithm approximates a marginal posterior distribution over the space of graphs and cluster indicators. 
