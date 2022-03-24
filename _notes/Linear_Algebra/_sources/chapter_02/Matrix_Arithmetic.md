# 2.1 Matrix Arithmetic

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Matrix
</b></font>

A matrix is A rectangular array of numbers. and each number from a matrix is called an entry of the matrix. Matrices are often denoted by uppercase letters: $A$, $B$, $C$,...
</div>

<font color='Blue'><b>Example</b></font>: $A$, $B$, and $C$ are matrices.
\begin{align*}
A=\begin{bmatrix} 1 & 0 \\ 2 & 1\end{bmatrix}_{2\times 2},~B=\begin{bmatrix} 1 & 3 & \frac{3}{2}\\ 2 & 1 & \sqrt{5}\end{bmatrix}_{2\times 3}
,~C=\begin{bmatrix} 1\\ 2 \\ -1 \end{bmatrix}_{3\times 1}
\end{align*}

<div class="alert alert-warning" role="alert">
<font size="+1"><b>
Remarks:
</b></font>

- A $m\times n$ matrix is a matrix with $m$ rows and $n$ columns. Also, when it is said a matrix has size $m\times n$, it has the same meaning.
- A **row matrix** is a matrix of size $1\times n$.
- Similarly, a **column matrix** is a matrix of size $n\times 1$.
</div>

<font color='Blue'><b>Example</b></font>: Matrices $A$, $B$, and $C$ above have sizes $2\times 2$, $2\times 3$, and $3\times 1$, respectively. Also, matrix $C$ above is an example of a column matrix.

<div class="alert alert-warning" role="alert">
<font size="+1"><b>
Remark:
</b></font>

We can identify each entry of a matrix by the row and column in which it lies. The rows are numbered from the top down, and the columns are
numbered from left to right. Thus, the **$(i,~j)$-entry** of a matrix is the number lying in row $i$ and column $j$.
</div>

<font color='Blue'><b>Example</b></font>: Consider 
\begin{align*}
D=\begin{bmatrix} 5 & 3 & 1\\ 0 & 2 & -1\end{bmatrix}.
\end{align*}

* The (1, 1)-entry of $D$ is 5.
* The (1, 2)-entry of $D$ is 3.
* The (1, 3)-entry of $D$ is 1.
* The (2, 1)-entry of $D$ is 0.
* The (2, 2)-entry of $D$ is 2.
* The (2, 3)-entry of $D$ is -1.

A special notation is commonly used for the entries of a matrix. If $A$ is an $m\times n$ matrix, and if the (i,j)-entry of A is denoted as $a_{ij}$, then $A$ is displayed as follows:

\begin{align*}
A=
\begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
a_{21} & a_{22} & \dots & a_{2n} \\
\vdots & \vdots &   & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn} \\
\end{bmatrix}
= \left[a_{i,j}\right]
\end{align*}

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Square Matrix
</b></font>

A matrix with the same number of rows and columns is called a **square matrix**.
</div>


<font color='Blue'><b>Example</b></font>: square matrices:

\begin{align*}
\begin{bmatrix} 1 & 0 \\ 2 & 1\end{bmatrix},\quad
\begin{bmatrix} 1 & 0 & 1\\ 2 & 1 & -1 \\ 3 & \sqrt{5} & \frac{5}{2}\end{bmatrix},\quad
\begin{bmatrix} 17 & 24 & 1 & 8 & 15\\ 23 & 5 & 7 & 14 & 16\\ 4 & 6 & 13 & 20 & 22\\ 10 & 12 & 19 & 21 & 3\\ 11 & 18 & 25 & 2 & 9\end{bmatrix}
\end{align*}

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Zero Matrix
</b></font>

A matrix in which all of its entries are zero is called a zero matrix. If a zero matrix has size $m\times n$, it is represented by $O_{m,n}$ (or simply just 0).
</div>


<font color='Blue'><b>Example</b></font>: zero matrices:
\begin{align*}
O_{2\times 2}=\begin{bmatrix} 0 & 0\\ 0 & 0\end{bmatrix},\quad
O_{2\times 3}=\begin{bmatrix} 0 & 0 & 0\\ 0 & 0 & 0\end{bmatrix},\quad
O_{3\times 1}=\begin{bmatrix} 0\\ 0\\ 0  \end{bmatrix}
\end{align*}

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Equal Matrices
</b></font>

Two matrices $A$ and $B$ are **equal** (written $A = B$) if and only if:

1. They have the same size.
1. Corresponding entries are equal.
</div>

<font color='Blue'><b>Example</b></font>:

\begin{align*}
\begin{bmatrix}  0 & 0 \\   0 & 0 \end{bmatrix} \neq \begin{bmatrix}  0 & 0 \\  0 & 0 \\  0 & 0 \end{bmatrix},
\quad
\begin{bmatrix}  1 & 2 \\   3 & 4 \end{bmatrix} \neq \begin{bmatrix}  2 & 1 \\  4 & 3 \end{bmatrix},
\quad
\begin{bmatrix}  1 & 2 \\   3 & 4 \end{bmatrix} = \begin{bmatrix}  1 & 2 \\  3 & 4 \end{bmatrix}.\end{align*}

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***