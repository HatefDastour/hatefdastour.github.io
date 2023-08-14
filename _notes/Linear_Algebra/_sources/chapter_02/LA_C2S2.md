# Addition of Matrices

We can add/subtract two matrices only if all matrices involved in the addition/subtraction need to have the **same size**.

`````{admonition} Matrix Addition
:class: tip

Assume that $A$ and $B$ are matrices of the same size, both having $m$ rows and $n$ columns. The summation of these matrices, denoted as $A + B$, is a new matrix calculated by adding the corresponding entries of matrices $A$ and $B$.

Mathematically, if $A$ and $B$ are $m\times n$ matrices, then the matrix $A + B$ is also an $m\times n$ matrix, and its entries are obtained as follows:

\begin{align*} (A + B)_{ij} = A_{ij} + B_{ij} \end{align*}

Where:
- $(A + B)_{ij}$ is the entry in the $i$-th row and $j$-th column of the matrix $A + B$.
- $A_{ij}$ is the entry in the $i$-th row and $j$-th column of matrix $A$.
- $B_{ij}$ is the entry in the $i$-th row and $j$-th column of matrix $B$.

To put it simply, to get the entry in the resulting matrix $A + B$ at position $(i,j)$, we add the corresponding entries from matrices $A$ and $B$ that are in the same position.


`````

<font color='Blue'><b>Example</b></font>:
For example, consider the following matrices:

\begin{align*} A = \begin{bmatrix}
2 & 4 \\
1 & 3
\end{bmatrix} \end{align*}

\begin{align*} B = \begin{bmatrix}
1 & 0 \\
2 & -1
\end{bmatrix} \end{align*}

The summation of matrices $A$ and $B$, denoted as $A + B$, will be:

\begin{align*} A + B = \begin{bmatrix}
2+1 & 4+0 \\
1+2 & 3+(-1)
\end{bmatrix}
= \begin{bmatrix}
3 & 4 \\
3 & 2
\end{bmatrix} \end{align*}

So, the resulting matrix $A + B$ is a $2\times 2$ matrix with entries obtained by adding the corresponding entries of matrices $A$ and $B$.


<font color='Blue'><b>Example</b></font>:
Let $A=\begin{bmatrix}  1 & -2 & 4\\ 3 & 0 & 7 \end{bmatrix}$
and $B=\begin{bmatrix}  6 & 2 & 4\\ -2 & 1 & -1 \end{bmatrix}$. Find $A+B$.

<font color='Green'><b>Solution</b></font>:

\begin{align*}
A+B &=\begin{bmatrix}  1 & -2 & 4\\ 3 & 0 & 7 \end{bmatrix}+\begin{bmatrix}  6 & 2 & 4\\ -2 & 1 & -1 \end{bmatrix}
\\ &
=\begin{bmatrix}  1+6 & -2+2 & 4+4\\ 3+(-2) & 0+1 & 7+(-1) \end{bmatrix}
\\ &
=\begin{bmatrix}  7 & 0 & 8\\ 1 & 1 & 6 \end{bmatrix}.
\end{align*}
***

<font color='Blue'><b>Example</b></font>:
If $C=\begin{bmatrix}  1 & -3 & 4\\ 0 & 1 & 2 \end{bmatrix}$
and $D=\begin{bmatrix}  1 & 1\\ 1 & 3 \end{bmatrix}$, we cannot have $C+D$ since $C$ is $2\times 3$ and $D$ is $2\times 2$.

```{admonition} Proposition - Properties of Matrix Addition:

Let $A$, $B$, and $C$ be matrices of the same size. Then,

- Commutative Law of Addition: $A+B = B+A$
- Associative Law of Addition: $(A+B)+C = A+(B+C)$
- Existence of an Additive Identity: There exists a zero matrix 0 such that $A+0 = A$
- Existence of an Additive Inverse: There exists a matrix $-A$ such that $A+(-A) = 0$

```
