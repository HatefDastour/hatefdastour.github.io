# 2.1.8 Inverses and Elementary Matrices

<div class="alert alert-info" role="alert">
<font size="+1"><b>
$B =UA$ Form
</b></font>

Let $A$ be an $m\times n$ matrix and let $B$ be the reduced row-echelon form of $A$. Then we can write $B =UA$ where U is the product of all elementary matrices representing the row operations done to $A$ to obtain $B$.
</div>

Suppose that an $m\times n$ matrix $A$ is carried to a matrix $B$ (written $A \to B$) by a series of $k$ elementary row operations.  Let $E_1$, $E_2$, \ldots, $E_k$ denote the corresponding elementary matrices.

1.  $B =UA$ where $U$ is an $m\times m$ invertible matrix.

2.  $U$ can be computed by $[~A~|~I_m~]\to[~B~|~U]$ using the operations
    carrying $A \to B$.

3.  $U = E _k E_{k-1} \ldots E_2 E_1$ where $E_1$, $E_2$, ..., $E_k$ are
    the elementary matrices corresponding (in order) to the elementary
    row operations carrying $A$ to $B$.

<font color='Blue'><b>Example</b></font>:
Let $A =\begin{bmatrix}2 & 3 & 1\\ 1 & 2 & 1\end{bmatrix}$. Find $B$, the reduced row-echelon form of $A$ and write it in the form $B =UA$.

<font color='Green'><b>Solution</b></font>:
Reduce the double matrix $[~A~|~I_2~]\to[~B~|~U]$ as follows:
\begin{align*}
[~A~|~I_2~] =& \left[\begin{array}{ccc|cc} 2 & 3 & 1 & 1 & 0\\ 1 & 2 & 1 & 0 & 1 \end{array}\right]
\\
{R_{1}\leftrightarrow R_{2}} \Rightarrow \quad &
\left[\begin{array}{ccc|cc} 1 & 2 & 1 & 0 & 1\\ 2 & 3 & 1 & 1 & 0 \end{array}\right]
\\
{-2R_{1}+R_{2}\rightarrow R_{2}} \Rightarrow \quad &
\left[\begin{array}{ccc|cc} 1 & 2 & 1 & 0 & 1\\ 0 & -1 & -1 & 1 & -2 \end{array}\right]
\\
{-R_{2}\rightarrow R_{2}} \Rightarrow \quad &
\left[\begin{array}{ccc|cc} 1 & 2 & 1 & 0 & 1\\ 0 & 1 & 1 & -1 & 2 \end{array}\right]
\\
{R_{1}-2R_{2}\rightarrow R_{1}} \Rightarrow \quad &
\left[\begin{array}{ccc|cc} {1} & 0 & -1 & 2 & -3\\ 0 & {1} & 1 & -1 & 2 \end{array}\right]=[~B~|~U].
\end{align*}
Hence,
\begin{equation*}
B=\begin{bmatrix}1 & 0 & -1\\ 0 & 1 & 1 \end{bmatrix}
\quad \text{and} \quad
U=\begin{bmatrix}2 & -3\\ -1 & 2 \end{bmatrix}.
\end{equation*}
***

Note that in the previous example,
```{image} ../Figures/fig2_00.png
:width: 600px
:align: center
```

and
\begin{equation*}
U=E_4E_3E_2E_1=\begin{bmatrix}2 & -3\\ -1 & 2\end{bmatrix}.
\end{equation*}

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
Letting $B = I$ gives $[~A~|~I~]\to[~I~|~U]$ where $I =UA$. Thus, with this assumption, $U = A^{-1}$, so we have
\begin{align*}[~A~|~I~]\to[~I~|~A^{-1}].\end{align*}

This is the matrix inversion algorithm. However, $A^{-1} =U = E_k E_{k-1} \ldots E_{2}E_{1}$ where $E_1$, $E_2$, \ldots, $E _k$ are the elementary matrices corresponding (in order) to the row operations carrying $A~\rightarrow~ I$. Hence
\begin{equation*}
A=\left(A^{-1}\right)^{-1}=\left(E_k E_{k-1} \ldots E_{2}E_{1}\right)^{-1}
=E_{1}^{-1} E_{2}^{-1} \ldots E_{k-1}^{-1} E_{k}^{-1}.
\end{equation*}
    
</div>

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: Product of Elementary Matrices
</b></font>
    
Let $A$ be an $n\times n$ matrix (square matrix). Then $A$ is invertible if and only if it can be written as a product of elementary matrices.
    
</div>

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
