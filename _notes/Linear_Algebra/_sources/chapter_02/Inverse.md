# Finding the Inverse of a Matrix

<div class="alert alert-block alert-success">
<font size="+1"><b>
Matrix Inverse Algorithm:
</b></font>
    
1. Form the augmented $n\times 2$ matrix $[~A~|~I~]$. Note that matrix $A$ is $n\times n$, but $[~A~|~I~]$ has double number of columns $n\times 2$.
1. If it is possible, perform row operations until you get an $n\times 2n$ matrix of the form $[~I~|~B~]$
1. Then, $B = A^{-1}$ and $A$ is **invertible**.
1. If it is impossible to row reduce to a matrix of the form $[~I~|~B~]$, then A has **no inverse**.    
</div>

<font color='Blue'><b>Example</b></font>: Find the inverse of $A=\begin{bmatrix}1 & 0 & 2 \\ 0 & 1 & 0 \\ 0 & 3 & -1\end{bmatrix}$  if it exists.

<font color='Green'><b>Solution</b></font>:
1.  Form the augmented $3\times 6$ matrix $[~A~|~I~]$ $$\begin{aligned}
    \left[\begin{array}{ccc|ccc} 1 & 0 & 2 & 1 & 0 & 0\\ 0 & 1 & 0 & 0 & 1 & 0\\ 0 & 3 & -1 & 0 & 0 & 1 \end{array}\right]\end{aligned}$$

2.  If possible do row operations until you obtain an $3\times 6$ matrix
    of the form $[~I~|~B~]$

\begin{align*}
[~A~|~I~]&=\left[\begin{array}{ccc|ccc} 1 & 0 & 2 & 1 & 0 & 0\\ 0 & 1 & 0 & 0 & 1 & 0\\ 0 & 3 & -1 & 0 & 0 & 1 \end{array}\right]\\
{-3R_{2}+R_{3}\rightarrow R_{3}} & \Rightarrow 
\left[\begin{array}{ccc|ccc} 1 & 0 & 2 & 1 & 0 & 0\\ 0 & 1 & 0 & 0 & 1 & 0\\ 0 & 0 & -1 & 0 & -3 & 1 \end{array}\right]
\\
{-R_{3}\rightarrow R_{3}} & \Rightarrow 
\left[\begin{array}{ccc|ccc} 1 & 0 & 2 & 1 & 0 & 0\\ 0 & 1 & 0 & 0 & 1 & 0\\ 0 & 0 & 1 & 0 & 3 & -1 \end{array}\right]
\\
{R_{1}-2R_{3}\rightarrow R_{1}} & \Rightarrow 
\left[\begin{array}{ccc|ccc} 1 & 0 & 0 & 1 & -6 & 2\\ 0 & 1 & 0 & 0 & 1 & 0\\ 0 & 0 & 1 & 0 & 3 & -1 \end{array}\right]=[~I~|~B~].
\end{align*}

Therefore,
\begin{align*}
A^{-1}=B =\begin{bmatrix}1 & -6 & 2\\ 0 & 1 & 0\\ 0 & 3 & -1\end{bmatrix}.
\end{align*}
***

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Inverses of Transposes and Products
</b></font>

1. For an an invertible matrix $A$, we have
\begin{align*}(A^T )^{-1} = (A^{-1} )^T.\end{align*}
1. For invertible matrices $A$ and $B$, we have
\begin{align*}(AB)^{-1} = B^{-1} A^{-1}.\end{align*}
1. For invertible matrices $A$, $B$ and $C$, we have
\begin{align*}\left(ABC \right)^{-1} = C^{-1}B^{-1}A^{-1}\end{align*} 
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Inverses of Transposes and Products
</b></font>

Let $A$ be a $n\times n$ matrix and $I$ be the identity matrix. Then,
1. I is invertible and $I^{-1} = I$
1. If $A$ is invertible, then $A^{-1}$ is also invertible and $A^{-1})^{-1} = A$.
1. If $A$ is invertible, then $A^{k}$ is also invertible and $(A^k )^{-1} = (A^{-1})^k$.
1. If $A$ is invertible and $p \neq 0$ ($p$ is a real number), then $pA$ is also invertible and $(pA)^{-1} = \frac{1}{p} A^{-1}$.
</div>

***
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
