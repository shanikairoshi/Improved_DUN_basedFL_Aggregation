## Improved_DUN_basedFL_Aggregation

This repository is the Python implementation of the paper: "Improving Federated Aggregation with Deep Unfolding Networks". submitted to IEEE network Letters, 2023

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

You can directly run these Python code.

1. main_env1.py: Code for setting I.
The distribution of data quantity is unbalanced across clients.
3. main_env2.py: Code for setting III
The clients in the system have different computational capabilities, which results in a variation in the number of epochs they can calculate during a round.
4. main_env3.py: Code for setting IV
Each client in the system has a communication capability skew, where the probability of transmitting the model parameters varies.


