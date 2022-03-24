# 2.1.7 Elementary Matrices

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Elementary Matrices and Row Operations
</b></font>

An $n\times n$ matrix $E$ is an **elementary matrix** if it can be obtained from the identity matrix $I_n$ through a **single row operation** (i.e.  switching the two rows, multiplying a row by some number and adding to another row, etc.). Those which involve switching rows of the identity matrix are called **permutation matrices**.
</div>



For example, the matrix
\begin{align*}
E=\begin{bmatrix}
    1 & 0 & 0 \\
    0 & 0 & 1 \\
    0 & 1 & 0
  \end{bmatrix}
\end{align*}

is the elementary matrix obtained from **switching the last two rows** of $I_{3}$. The matrix
\begin{align*}
E=\begin{bmatrix}
    3 & 0 & 0 \\
    0 & 1 & 0 \\
    0 & 0 & 1
  \end{bmatrix}
\end{align*}
is the elementary matrix obtained from **multiplying the first row** of $I_{3}$ by 3. The matrix
\begin{align*}
E=\begin{bmatrix}
    1 & 0 \\
    5 & 1 \\
  \end{bmatrix}
\end{align*}
is the elementary matrix obtained from **adding $5$ times the first row to the second row** of $I_{2}$.

<div class="alert alert-block alert-success">
    
* **Multiplication by an Elementary Matrix and Row Operations:**
Let $E$ be an elementary matrix obtained by using the preferred row operation on the identity matrix and $A$ be a matrix. Then, the product $EA$ applies the same row operations on the matrix $A$.

* **Action of Permutation Matrix</strong>:**
Let $P^{ij}$ be a permutation matrix (an elementary matrix which involves switching the $i^{\text{th}}$ and the $j^{\text{th}}$ rows). $P^{ij}A$ is a matrix obtained from $A$ by switching the $i^{\text{th}}$ and the $j^{\text{th}}$ rows.
    
</div>

<font color='Blue'><b>Example</b></font>:
Let
\begin{align*}
P^{23}=\begin{bmatrix}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{bmatrix},
~A=\begin{bmatrix}
1 & 2 \\
3 & 4 \\
5 & 6
\end{bmatrix}.
\end{align*}
Find $B$ where $B = P^{23}A$

<font color='Green'><b>Solution</b></font>:
$B$ can be obtained from switching the last two rows of matrix $A$. Therefore,
\begin{align*}
B=\begin{bmatrix}1 & 2 \\
5 & 6 \\
3 & 4
\end{bmatrix}
\end{align*}
***

<div class="alert alert-block alert-success">

**Multiplication by a Scalar and Elementary Matrices:**
Let $E(k,i)$ be the elementary matrix corresponding to the row operation in which the $i^{\text{th}}$ row is multiplied by the scalar $k$ (nonzero). Then
\begin{align*}
E(k,i)A = B
\end{align*}
where $B$ is obtained from $A$ by multiplying the $i^{\text{th}}$ row of $A$ by $k$.

**Action of Permutation Matrix:**
Let $E(k\times \, i+ \, j)$ denote the elementary matrix obtained from $I$ by adding $k$ times the $i^{\text{th}}$  row to the $j^{\text{th}}$ . Then
\begin{align*}
E(k\times \, i+ \, j) A = B
\end{align*}
where $B$ is obtained from $A$ by adding $k$ times the $i^{\text{th}}$ row to the $j^{\text{th}}$ row of A.
</div>

<font color='Blue'><b>Example</b></font>:
Let
\begin{align*}
A=\begin{bmatrix}
1 & 2 \\
3 & 4 \\
5 & 6
\end{bmatrix}.
\end{align*}
Find $B = E(3,1)A$ and $C = E(4\times \, 2+ \, 3)A$

<font color='Green'><b>Solution</b></font>:
$B$ can be obtained from multiplying the first row of matrix $A$ by 3 and replacing it with the first row of $A$. Therefore,
$B=\begin{bmatrix}3 & 6 \\3 & 4 \\5 & 6\end{bmatrix}$.

Moreover, $C$ can be obtained from multiplying the second row of matrix $A$ by 4 and adding it to the last row of $A$. Therefore,
$C=\begin{bmatrix}1 & 2 \\3 & 4 \\17 & 22\end{bmatrix}$.
***

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Elementary Matrices and Inverses
</b></font>
    
Every elementary matrix is invertible and its inverse is also an elementary matrix.
    
</div>

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
