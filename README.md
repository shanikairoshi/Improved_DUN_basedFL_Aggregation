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


## Results

*  Based on the provided figures, it is evident that our proposed method, which incorporates regularization penalties and leverages a deep unfolding-based weighting strategy, achieves superior accuracy, lower losses and proper unbiasedness compared to other methods.
*  The precise weighting strategy employed by our method contributes to these improved performance metrics.
![image](https://github.com/shanikairoshi/Improved_DUN_basedFL_Aggregation/assets/19671763/3d18bd26-2f4e-4d1b-a69a-cffb6d688349)
![image](https://github.com/shanikairoshi/Improved_DUN_basedFL_Aggregation/assets/19671763/b799e17b-f766-4736-a68d-32ce52ae6dcb)

Furthermore, we can achieve these results under low computational power due to lower training iterations. The following table shows the complexity reduction aas the percentage.

![image](https://github.com/shanikairoshi/Improved_DUN_basedFL_Aggregation/assets/19671763/08b577d9-1fe3-4c82-835b-d21b195b0c0b)


## Acknowledgment
- Original method, which is called DUW_fedAvg, extracted from [this paper](https://arxiv.org/abs/2212.12191#:~:text=Device%20and%20statistical%20heterogeneity%20of%20the%20participating%20clients,model%20with%20high%20accuracy%20on%20uniform%20test%20data.)

- And we proposed a new approach that can achieve more accuracy and unbiasedness in FL aggregation.

- Datasets are extracted from MNIST by using [this repository](https://github.com/a-nakai-k/DeepUnfolding-based-FL).





