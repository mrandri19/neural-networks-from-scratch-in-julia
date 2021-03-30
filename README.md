# Neural networks from scratch in Julia

|![image](https://user-images.githubusercontent.com/8144521/113006870-04585b80-9176-11eb-9860-9268ff64ebb6.png)|![image](https://user-images.githubusercontent.com/8144521/113006884-07ebe280-9176-11eb-93b5-3892d0111142.png)|
|:-------------------------------------------------------:|:-------------------------------------:|
| Training and test accuracy evolution, epoch after epoch | Test predictions of the final network |

[Nbviewer Link](https://nbviewer.jupyter.org/github/mrandri19/neural-networks-from-scratch-in-julia/blob/main/MLP.ipynb) to the `MLP.ipynb` file, containing the lastest updates.

This project consists of a fully from-scratch implementation of a fully-connected neural network (Multi Layer Perceptron) in Julia.

## Performance

It achieves `94.7%` test accuracy on the MNIST dataset after less than 30 seconds of training.
The network architecture used to obtain these results consists of 784 input neurons, 30 hidden neurons, 10 output neurons, for a total of 23830 learned parameters.

## Features

- Almost zero extra allocations in the forward and backward passes. Just the necessary matrices for intermediate results, and most results are computed in-place
- Mean Squared Error Loss and Categorical Cross Entropy Loss
- Vectorized across minibatches

## References

This was build following the excellent [Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/) by Michael Nielsen.
