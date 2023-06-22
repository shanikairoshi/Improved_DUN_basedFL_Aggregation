## Improved_DUN_basedFL_Aggregation

This repository is the Python implementation of the paper: titled "Improving Federated Aggregation with Deep Unfolding Networks", which is inspired by "DEEP UNFOLDING-BASED WEIGHTED AVERAGING FOR FEDERATED LEARNING UNDER HETEROGENEOUS ENVIRONMENTS"

## Requirements

This code is implemented in 
Python 3.9, using matplotlib and numpy.

## System Setup

The number of clients and rounds were fixed to K = 5, M = 100, and T = 10, respectively. We
used three characteristic training datasets extracted from the MNIST dataset.

1. Setting 01: This contains imbalanced data introducing statistical heterogeneity
2. Setting 02: This setting skew the computational capabilities by adjusting several epochs while keeping balanced data.
3. Setting 03: This setting skew communication capabilities while maintaining balanced data.



## Usage

You can directly run these python code.

1. main_env1.py: Code for setting I.
2. main_env2.py: Code for setting III containing computational capability skew. The number of epochs that can calculate during a round varies across clients.
3. main_env3.py: Code for setting IV containing communication capability skew. Each client can transmit the model parameters only with a certain probability.


