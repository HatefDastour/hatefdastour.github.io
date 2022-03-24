# 2.1.5 The Identity and Inverses

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Main Diagonal
</b></font>

The entries $a_{11},~a_{22},~a_{33},\ldots$ form the main diagonal.
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Symmetric and Skew Symmetric Matrices
</b></font>

An $n\times n$ matrix $A$ is
* **symmetric** if $A = A^T$. 
* **skew-symmetric** if $A = -A^T$.

</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
Note that a symmetric matrix has to be a square matrix. If a symmetric $A$ is $m\times n$, then $A^T$ is $n\times m$, so $A=A^T$ forces $n=m$. 
</div>

<font color='Blue'><b>Example</b></font>: Examples of symmetric and skew symmetric matrices.


-   $\begin{bmatrix}1 & 2\\ 2 & 1\end{bmatrix}$ (Symmetric),

-   $\begin{bmatrix}1 & 2 & 3\\ 2 & 1 & 3\\ 3 & 3 & 1\end{bmatrix}$ (Symmetric),

-   $\begin{bmatrix} 0 & 2 & 3 & 13\\ -2 & 0 & 10 & 8\\ -3 & -10 & 0 & 12\\ -13 & -8 & -12 & 0 \end{bmatrix}$
    (Skew-symmetric),

-   $\begin{bmatrix}0 & 24 & 1 & 8 & 15\\ -24 & 0 & 7 & 14 & 16\\ -1 & -7 & 0 & 20 & 22\\ -8 & -14 & -20 & 0 & 3\\ -15 & -16 & -22 & -3 & 0\end{bmatrix}$
    (Skew-symmetric).

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
The entries on the main diagonal of a skew-symmetric matrix are **zero**. 
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
The Identity matrix
</b></font>

The identity matrix is (always) a square matrix that there are ones on its main diagonal and zeroes elsewhere, and it is shown with $I_n$ for $n\geq 1$.
</div>

<font color='Blue'><b>Example</b></font>: Some identity matrices of various sizes

\begin{align*}
I_1=\begin{bmatrix} 1 \end{bmatrix},~I_2=\begin{bmatrix} 1 & 0\\ 0 & 1 \end{bmatrix}~I_3=\begin{bmatrix} 1 & 0 & 0\\ 0 & 1 & 0\\ 0 & 0 & 1 \end{bmatrix},\ldots
\end{align*}

<div class="alert alert-block alert-success">
<font size="+1"><b>
Lemma: Multiplication by the Identity Matrix
</b></font>
    
Assume that $A$ is an $m\times n$ matrix and $I_n$ is the $n\times n$ identity matrix. Then
\begin{align*}
AI_n = A.
\end{align*}
If $I_m$ is the $m\times m$ identity matrix, then 
\begin{align*}
I_m A = A.
\end{align*}
In other words, it is the only matrix such that when multiplied by itself the result is itself.
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
We generally use $I$ instead of $I_m$ and $I_n$.
</div>

<div class="alert alert-block alert-success">
<font size="+1"><b>
The Inverse of a Matrix
</b></font>
    
A square matrix $A$ is said that have an inverse $A^{-1}$ (read it $A$ inverse) if and only if 
\begin{align*}
AA^{-1} = A^{-1} A = I_n
\end{align*}

If matrix $A$ has an inverse, then the matrix $A$ is
called **invertible**.
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Uniqueness of Inverse
</b></font>
If matrix $A$ has an inverse, then its inverse is unique. That is, if $B$ and $C$ are both inverses of $A$, then $B =C$.
</div>

<font color='Blue'><b>Example</b></font>: Show that $A=\begin{bmatrix} 1 & 2\\ 0 & 1 \end{bmatrix}$ is the inverse of $B=\begin{bmatrix} 1 & -2\\ 0 & 1 \end{bmatrix}$.

\<font color='Green'><b>Solution</b></font>:
We need to show that $AB = I$ and $ BA = I$. Therefore,
\begin{align*}
AB &=\begin{bmatrix}1 & 2\\ 0 & 1\end{bmatrix}
\begin{bmatrix}1 & -2\\ 0 & 1\end{bmatrix}=
\begin{bmatrix}1 & 0\\ 0 & 1\end{bmatrix} & \surd
\\
BA &=\begin{bmatrix} 1 & -2\\ 0 & 1 \end{bmatrix}
\begin{bmatrix} 1 & 2\\ 0 & 1 \end{bmatrix}=
\begin{bmatrix}1 & 0\\ 0 & 1\end{bmatrix} & \surd
\end{align*}
***

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
1.  Not every (square) matrix is invertible. For example,
    $\begin{bmatrix} 1 & 1 \\ 1 & 1 \end{bmatrix}$ (See page 72 of the
    textbook for the reason).

2.  Zero matrix has no inverse.
    
</div>

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
