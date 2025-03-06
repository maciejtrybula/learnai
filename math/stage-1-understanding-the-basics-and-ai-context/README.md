# 🎓 Stage 1: Understanding the Basics and AI Context



## Fundamentals of Mathematics for AI

Artificial Intelligence (AI), particularly Machine Learning (ML) and Deep Learning (DL), relies heavily on mathematics. The key areas are:

* **Linear Algebra** – describes how neural networks work and how data operations are performed.
* **Calculus** – enables model optimization through algorithms like backpropagation.
* **Statistics and Probability Theory** – helps in modeling data, analyzing results, and making decisions under uncertainty.



### Linear Algebra - The Foundation of AI

#### Vectors and Matrices

**Vector** – a collection of numbers arranged in a single row or column, e.g.:

* Row vector:

$$
\begin{bmatrix} 1 & 2 & 3 \end{bmatrix}
$$

* Column vector:

$$
\begin{bmatrix} 1 \\ 2 \\ 3 \end{bmatrix}
$$

**Matrix** – a table of numbers, e.g.:&#x20;



$$
\begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}
$$

**Matrix-vector multiplication** (a linear transformation) is essential for propagating data through neural network layers.



Dot Product and Matrix Multiplication

**Dot product** of two vectors:

$$
a \cdot b = a_1b_1 + a_2b_2 + \cdots a_nb_n
$$

Used in classifiers such as perceptrons.

**Matrix multiplication** (important for neural networks):

$$
C = A \times B
$$

Each value in the resulting matrix is a combination of the rows and columns of the input matrices.



#### Matrices in AI

* **Weight matrices** – define the strength of connections between neurons in neural networks.
* **Matrix transposition** – swapping rows with columns



$$
A^T = \begin{bmatrix} 1 & 3 \\ 2 & 4 \end{bmatrix}
$$

* **Identity and inverse matrices** – used in solving systems of equations and data transformations.

#### Vector Spaces and Transformations

* **Vector space** – a collection of vectors that can be added and scaled.
* **Eigenvalues and eigenvectors** – crucial in Principal Component Analysis (PCA), which reduces data dimensionality.



### Calculus - Optimizing AI Models

#### Derivatives and Their Interpretation

* The **derivative** of a function measures how its value changes with small input variations:



$$
f'(x) =\lim _{x \to 0 } \frac {f(x+h) - f(x)} {h}
$$

In AI, this is used to find the minimum of a cost function, optimizing the model’s parameters.

#### Gradient and Its Role in AI

* **Gradient** – a vector of partial derivatives showing the direction of the steepest function change:



$$
\nabla f(x,y) = \begin{bmatrix} \frac {\partial f} {\partial x} \\ \frac {\partial f} {\partial y} \end{bmatrix}
$$

* **Backpropagation** – uses gradients to update weights in neural networks.

#### Model Optimization

* **Gradient Descent Algorithm**:



$$
w := - \alpha \nabla L (w)
$$

where 𝛼 is the learning rate, and 𝐿 ( 𝑤 ) is the loss function.

* **Adam, RMSProp** – advanced optimizers used in deep learning.



### Statistics and Probability Theory

#### Basic Concepts

* **Mean, median, variance** – describe the distribution of data.
* **Normal distribution (Gaussian)** – common in AI models.
* **Conditional probability** – key in predictive models.

#### Bayes’ Theorem

* Updates beliefs based on new data:



$$
P(A|B) = \frac {P(B|A)P(A)} {P(B)}
$$

* Used in Bayesian classifiers.

#### Sampling and Estimation

* **Linear regression** – a fundamental predictive model.
* **Statistical tests** – verify hypotheses in data analysis.
