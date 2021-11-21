# ORCCA
Optimal Randomized Canonical Correlation Analysis

This project is for the python version of ORCCA algorithm.

It depends on Numpy for matrix calculation and works with any CCA calculation package. Here we recommend 

cca zoo
https://github.com/jameschapman19/cca_zoo

for CCA calculation as it provides several other CCA algorithms that can be used in algorithm comparison. Please feel free to delete the cca_zoo dependency in the manuscript by deleting line2 and ORCCA_cor function.

# Some working exmaples for using ORCCA:

1. Generate ORCCA mapping for a given pair of dataset X and Y with 5 reselected random features

sample = ORCCA(X,Y,width1=0.1)

sample.ORCCA_mapping(m=5)

2. Calculate the canonical correlations for a given pair of dataset X and Y with 5 reselected random features

sample = ORCCA(X,Y,width1=0.1)

sample.ORCCA_cor(m=5)

