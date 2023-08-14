# Scalar Multiplication of Matrices


`````{admonition} Scalar Multiplication of Matrices
:class: tip

Let $A =\left[a_{ij}\right]$ be a matrix, and $k$ is a scalar (a number). The scalar multiplication of the matrix $A$ by the scalar $k$, denoted as $kA$, is a new matrix obtained by multiplying each entry of $A$ by the scalar $k$.

Mathematically, if $A$ is an $m\times n$ matrix, then $kA$ is also an $m\times n$ matrix, and its entries are calculated as follows:

\begin{align*} (kA)_{ij} = k \cdot a_{ij} \end{align*}

Where:
- $(kA)_{ij}$ is the entry in the $i$-th row and $j$-th column of the matrix $kA$.
- $a_{ij}$ is the entry in the $i$-th row and $j$-th column of the original matrix $A$.
- $k$ is the scalar (a constant number).

To put it simply, to get the entry in the resulting matrix $kA$ at position $(i,j)$, we multiply the corresponding entry in matrix $A$ by the scalar $k$.

`````
<font color='Blue'><b>Example</b></font>:  For example:

Let's consider the following matrix:

\begin{align*} A = \begin{bmatrix}
2 & 4 \\
1 & 3
\end{bmatrix} \end{align*}

If we multiply this matrix by the scalar $k = 3$, the resulting matrix $kA$ will be:

\begin{align*} kA = 3 \cdot \begin{bmatrix}
2 & 4 \\
1 & 3
\end{bmatrix} = \begin{bmatrix}
3\cdot2 & 3\cdot4 \\
3\cdot1 & 3\cdot3
\end{bmatrix} = \begin{bmatrix}
6 & 12 \\
3 & 9
\end{bmatrix} \end{align*}

So, the resulting matrix $kA$ is a $2\times 2$ matrix, and each entry is obtained by multiplying the corresponding entry in matrix $A$ by the scalar $k = 3$.

<font color='Blue'><b>Example</b></font>: If $A=\begin{bmatrix}1 & 2 \\ 3 & 4\end{bmatrix}$, find $cA$ and $-A$.

<font color='Green'><b>Solution</b></font>:

1. **$3A$**:
   We have the matrix $A$ as:
   \begin{align*} A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} \end{align*}

   To find $3A$, we multiply each entry of matrix $A$ by the scalar $3$:
   \begin{align*} 3A = 3 \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} = \begin{bmatrix} (3)(1) & (3)(2) \\ (3)(3) & (3)(4) \end{bmatrix} = \begin{bmatrix} 3 & 6 \\ 9 & 12 \end{bmatrix} \end{align*}

   In this case, every entry in the resulting matrix $3A$ is obtained by multiplying the corresponding entry in matrix $A$ by the scalar $3$.

2. **$-A$**:
   We have the same matrix $A$ as above:
   \begin{align*} A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} \end{align*}

   To find $-A$, we multiply each entry of matrix $A$ by the scalar $-1$ (which is the same as negating each entry):
   \begin{align*} -A = (-1) \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} = \begin{bmatrix} (-1)(1) & (-1)(2) \\ (-1)(3) & (-1)(4) \end{bmatrix} = \begin{bmatrix} -1 & -2 \\ -3 & -4 \end{bmatrix} \end{align*}

   In this case, every entry in the resulting matrix $-A$ is obtained by multiplying the corresponding entry in matrix $A$ by the scalar $-1$ (i.e., negating each entry).

Scalar multiplication of a matrix involves multiplying each entry of the matrix by the scalar, resulting in a new matrix with the same dimensions. It's a straightforward operation and is a fundamental concept in linear algebra.
***

<div class="alert alert-warning" role="alert">
<font size="+1"><b>
Remark:
</b></font>
    
The subtraction of matrices is comparable to the addition of matrices (since $A-B=A+(-B)$). However, subtraction is not commutative which means, in general, for two matrices $A$ and $B$

\begin{align*}
A-B\neq B-A.
\end{align*}
</div>

```{admonition} Proposition - Properties of Scalar Multiplication:

- Distributive Law over Matrix Addition: $k(A+B) = kA+kB$,
- Distributive Law over Scalar Addition: $(k+ p)A = kA+ pA$,
- Associative Law for Scalar Multiplication: $k(pA) = (kp)A$,
- Rule for Multiplication by 1: $1A = A$.

```
