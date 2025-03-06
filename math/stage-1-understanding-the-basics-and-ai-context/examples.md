---
icon: code
---

# Examples

## **1 Linear Algebra in AI**

### **1.1 Vectors and Matrices using NumPy**

```python
import numpy as np

# Creating a vector
v = np.array([1, 2, 3])
print("Vector v:", v)

# Creating a matrix
A = np.array([[1, 2], [3, 4]])
print("Matrix A:\n", A)

# Matrix-vector multiplication
result = np.dot(A, v[:2])  # Multiplying A with first two elements of v
print("Matrix-vector multiplication result:", result)
```

### **1.2 Dot Product and Matrix Multiplication**

```python
# Dot product of two vectors
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
dot_product = np.dot(a, b)
print("Dot product:", dot_product)

# Matrix multiplication
B = np.array([[5, 6], [7, 8]])
matrix_mult = np.dot(A, B)
print("Matrix multiplication result:\n", matrix_mult)
```

***

## **2 Calculus for Optimization**

### **2.1 Derivatives with SymPy**

```python
from sympy import symbols, diff

x = symbols('x')
f = x**2 + 3*x + 2  # Define function f(x) = x^2 + 3x + 2
derivative = diff(f, x)  # Compute the derivative
print("Derivative of f(x):", derivative)
```

### **2.2 Gradient Descent Example**

```python
import numpy as np

# Function to minimize: f(x) = (x-3)^2
def f(x):
    return (x - 3)**2

# Derivative (Gradient)
def grad_f(x):
    return 2 * (x - 3)

# Gradient Descent
learning_rate = 0.1
x = np.random.randn()  # Random initial point

for i in range(10):  # 10 iterations
    x = x - learning_rate * grad_f(x)  # Gradient descent update
    print(f"Iteration {i+1}, x: {x}, f(x): {f(x)}")
```

***

## **3 Probability and Statistics in AI**

### **3.1 Gaussian Distribution**

```python
import numpy as np
import matplotlib.pyplot as plt

mean = 0  # Mean of the distribution
std_dev = 1  # Standard deviation
samples = np.random.normal(mean, std_dev, 1000)  # Generate 1000 samples

plt.hist(samples, bins=30, density=True, alpha=0.6, color='b')
plt.title("Gaussian Distribution")
plt.show()
```

### **3.2 Bayes' Theorem Calculation**

```python
# Bayes' Theorem: P(A|B) = (P(B|A) * P(A)) / P(B)
def bayes_theorem(p_a, p_b_given_a, p_b):
    return (p_b_given_a * p_a) / p_b

p_a = 0.1  # Prior probability of A
p_b_given_a = 0.8  # Likelihood of B given A
p_b = 0.2  # Total probability of B

posterior = bayes_theorem(p_a, p_b_given_a, p_b)
print("Posterior probability P(A|B):", posterior)
```
