# Fully-Recurrent-Network


## Exercise 1: Data generation

There are two classes, both occurring with probability 0.5. There is one input unit. Only the first sequence element conveys relevant information about the class. Sequence elements at positions $t > 1$ stem from a Gaussian with mean zero and variance 0.2. The first sequence element is 1.0 (-1.0) for class 1 (2). Target at sequence end is 1.0 (0.0) for class 1 (2)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Exercise 2: Gradients for the network parameters

<img width="1162" alt="image" src="https://github.com/user-attachments/assets/bfac6b45-6f30-4e54-97ba-0c65eeaf62b7">

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Exercise 3: The backward pass
Write a function `backward` that takes a model `self` as argument. The function should compute the gradients of the loss with respect to all model parameters and store them to `self.dW`, `self.dR`, `self.dV`, respectively.
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Exercise 4: Gradient checking

<img width="1408" alt="image" src="https://github.com/user-attachments/assets/15dbf2e7-3dcd-4ee4-b971-e06b0e020657">

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Exercise 5: Parameter update

Write a function `update` that takes a model `self` and a float argument `eta`, which represents the learning rate. The method should implement the gradient descent update rule $\theta \gets \theta - \eta \nabla_{\theta}L$ for all model parameters $\theta$.
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Exercise 6: Network training

Train the fully recurrent network with 32 hidden units. Start with input sequences of length one and tune the learning rate and the number of update steps. Then increase the sequence length by one and tune the hyperparameters again. What is the maximal sequence length for which the fully recurrent network can achieve a performance that is better than random? Visualize your results.
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
