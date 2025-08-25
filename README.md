# Simple Neural Network from Scratch (Backpropagation)

This project implements a **basic feedforward neural network** with backpropagation in Python **without using external libraries like TensorFlow or PyTorch**.  

It is based on the classic example from *Neural Networks and Deep Learning by Michael Nielsen*.

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
