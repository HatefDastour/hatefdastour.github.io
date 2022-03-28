# 2.1.2 Scalar Multiplication of Matrices


<div class="alert alert-info" role="alert">
<font size="+1"><b>
Scalar Multiplication of Matrices
</b></font>

If $A =\left[a_{i,j}\right]$ and $k$ is a scalar (a number), then $kA = \left[k~a_{i,j}\right]$.
</div>


<font color='Blue'><b>Example</b></font>: If $A=\begin{bmatrix}1 & 2 \\ 3 & 4\end{bmatrix}$, find $cA$ and $-A$.

<font color='Green'><b>Solution</b></font>:

\begin{align*}
3A&=\begin{bmatrix}1 & 2 \\ 3 & 4\end{bmatrix}=\begin{bmatrix}(3)(1) & (3)(2) \\ (3)(3) & (3)(4)\end{bmatrix}
=\begin{bmatrix}3 & 6\\ 9 & 12\end{bmatrix},\\
-A&=\begin{bmatrix}1 & 2 \\ 3 & 4\end{bmatrix}=\begin{bmatrix}(-1)(1) & (-1)(2) \\ (-1)(3) & (-1)(4)\end{bmatrix}
=\begin{bmatrix}-1 & -2\\ -3 & -4\end{bmatrix}.\end{align*}
***

<div class="alert alert-warning" role="alert">
<font size="+1"><b>
Remark:
</b></font>
    
The subtraction of matrices is similar to the addition of matrices (since $A-B=A+(-B)$). However, subtraction is not commutative which means, in general, for two matrices $A$ and $B$

\begin{align*}
A-B\neq B-A.
\end{align*}
</div>

<div class="alert alert-block alert-info">
<font size="+1"><b>
Proposition - Properties of Scalar Multiplication:
</b></font>
    
<p><span class="math display">\[\begin{array}{llc}
\bullet &\text{Distributive Law over Matrix Addition:} & k(A+B) = kA+kB, \\
\bullet &\text{Distributive Law over Scalar Addition:} & (k+ p)A = kA+ pA, \\
\bullet &\text{Associative Law for Scalar Multiplication:} & k(pA) = (kp)A,\\
\bullet &\text{Rule for Multiplication by 1:} & 1A = A.
\end{array}\]</span></p>
    
</div>