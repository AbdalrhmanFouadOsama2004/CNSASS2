# Simple Neural Network from Scratch (Backpropagation)

## Summary
This project implements a simple **feedforward neural network** with one hidden layer and trains it using **backpropagation**.  
It is coded entirely from scratch in Python, without using machine learning libraries, to demonstrate the math behind neural networks.  
The network learns to approximate the mapping from `[0.05, 0.10]` to `[0.01, 0.99]`.

---

## 📌 Project Description
- Input layer: 2 neurons  
- Hidden layer: 2 neurons  
- Output layer: 2 neurons  

The network is trained using **gradient descent** with the sigmoid activation function and its derivative.  
The training runs for 10,000 epochs on the following example:

- **Inputs:** `[0.05, 0.10]`  
- **Expected output:** `[0.01, 0.99]`  

---

## ⚙️ How it works
1. **Forward pass**  
   - Compute hidden layer activations using weights + bias  
   - Compute output layer activations  

2. **Backward pass (Backpropagation)**  
   - Compute output error  
   - Update output layer weights and biases  
   - Propagate error to hidden layer  
   - Update hidden layer weights and biases  

3. **Repeat** for 10,000 epochs with a learning rate of `0.5`.

---

## 🧮 Activation Function
The network uses the **Sigmoid function**:

\[
\sigma(x) = \frac{1}{1 + e^{-x}}
\]

and its derivative:

\[
\sigma'(x) = x \cdot (1 - x)
\]

---

## 📊 Final Result
After training, the network prints the **final output values**:

```python
Final Output after training:
[ y1, y2 ]
