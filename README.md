# Simple Neural Network from Scratch
Building AI course project

## Summary
This project builds a simple feedforward neural network with one hidden layer and trains it using backpropagation.  
The goal is to explain how forward and backward passes work in practice, without using machine learning libraries.


---

## Project Description
- Input layer: 2 neurons  
- Hidden layer: 2 neurons  
- Output layer: 2 neurons  

The network is trained on a simple dataset:  
- **Inputs:** `[0.05, 0.10]`  
- **Expected outputs:** `[0.01, 0.99]`  

Training is done for 10,000 epochs with a learning rate of 0.5.

---

## How it works
1. **Forward pass** – compute hidden and output activations  
2. **Backward pass** – calculate errors and update weights using gradients  
3. **Repeat** until the output approximates the expected values  

---

## Activation Function
The Sigmoid function is used:

\[
\sigma(x) = \frac{1}{1 + e^{-x}}
\]

and its derivative:

\[
\sigma'(x) = x \cdot (1 - x)
\]

---

## Results
After training, the network produces outputs close to the expected `[0.01, 0.99]`.  
This shows that even a simple two-layer neural network can learn via backpropagation.
