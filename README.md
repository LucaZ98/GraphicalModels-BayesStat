# GraphicalModels-BayesStat
Project for the course Bayesian Statistics at Politecnico di Milano.

## Main goal
The aim of this project is to develop Bayesian methods for the analysis of multivariate categorical data. In particular, we are interested in inferring dependence relations between categorical variables, also accounting for possible heterogeneity related to latent clustering structures in the data.

## Personal contribution
I considered mixtures of graphical models to account for possible heterogeneous dependence relations among subjects, which can be linked to a latent clustering structure of the data. We base our model formulation on a Dirichlet Process (DP) mixture of graphical models, a representation that allows us to implement a MCMC scheme for
posterior inference on clustering and graphs as follows:

- as a first step we update cluster indicators (and implicitly the total number of clusters) through a Gibbs sampling scheme which sequentially samples
each cluster indicator from its full conditional distribution;
- secondly, we update the graph of each cluster through a Metropolis-Hastings step where a new graph is proposed from a suitable proposal distribution and then accepted with a certain probability.
