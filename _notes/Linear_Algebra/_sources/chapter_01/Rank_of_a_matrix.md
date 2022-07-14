# 1.2.4 Rank of a matrix

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Rank of a Matrix
</b></font>

The rank of matrix $A$ is the number of leading 1s in the reduced row-echelon form (RREF) of the matrix $A$.
</div>


<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem:
</b></font>
    
Consider following system of equations with $m$ equations in $n$ variables
\begin{align*}
\begin{cases}
a_{11}x_1+\ldots+a_{1n}x_{n}=0\\
a_{21}x_1+\ldots+a_{2n}x_{n}=0\\
\vdots \\
a_{m1}x_1+\ldots+a_{mn}x_{n}=0.
\end{cases}
\end{align*} 
Suppose that the rank of the augmented matrix is $r$. Then

* If $r<n$ , the system has **infinitely many solutions**.
* If $r = n$ , the system has **a unique solution**.
</div>


<font color='Blue'><b>Example</b></font>: Consider the following system of equations 

$$
\begin{cases}
x_{1}-2\,x_{2}-x_{3}=1\\ 2\,x_{1}-4\,x_{2}+x_{3}=5\\ x_{1}-2\,x_{2}+2\,x_{3}=4
\end{cases}
$$

<font color='Green'><b>Solution</b></font>: The corresponding augmented matrix is

\begin{align*}
\left[\begin{array}{ccc|c} 1 & -2 & -1 & 1\\ 2 & -4 & 1 & 5\\ 1 & -2 & 2 & 4 \end{array}\right].\end{align*}

From previous examples, we know the RREF of this matrix is

\begin{align*}
\left[\begin{array}{ccc|c} {1} & -2 & 0 & 2\\ 0 & 0 & {1} & 1\\ 0 & 0 & 0 & 0 \end{array}\right]\end{align*}

It can be seen that $r=Rank(A)=2$ and the number of variables is $n=3$.
From the above theorem, we know that if $r < n$ , the system has
**infinitely many solutions**.
***

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Linear Combinations
</b></font>

Let $X_1,~X_2,~\ldots,~X_n$, $V$ be column matrices (each of them consists of only one column). Then, $V$ is said to be a **linear combination** of the columns $X_1,~X_2,~\ldots,~X_n$ if there exist scalars, $a_1,~a_2,~\ldots,~a_n$ such that

\begin{align*}
V=a_1X_1+a_2X_2+\ldots+a_nX_n.
\end{align*}

In other words, $V$ is a **linear combination** of the columns $X_1,~X_2,~\ldots,~X_n$ if it can be expressed in terms of those column matrices.
</div>

<font color='Blue'><b>Example</b></font>:
Let $X_1=\begin{bmatrix} 1 \\ 2 \\ 3\end{bmatrix}$ and
$X_2=\begin{bmatrix} 2 \\ 1 \\ 1\end{bmatrix}$. Then

\begin{align*}
V&=2\begin{bmatrix} 1 \\ 2 \\ 3\end{bmatrix}+3\begin{bmatrix} 2 \\ 1 \\ 1\end{bmatrix}
\\ &
=\begin{bmatrix} (2)(1) \\ (2)(2) \\ (2)(3)\end{bmatrix}+3\begin{bmatrix} (3)(2) \\ (3)(1) \\ (3)(1)\end{bmatrix}
\\ &
=\begin{bmatrix} 2\\ 4\\ 6\end{bmatrix}+3\begin{bmatrix} 6\\ 3\\ 3\end{bmatrix}
=\begin{bmatrix}8\\ 7\\ 9\end{bmatrix}\end{align*}

is a linear
combination of $X_1$ and $X_2$.
***

<font color='Blue'><b>Example</b></font>:
Find all values of $r$ so that $V=\begin{bmatrix}1\\r\\0\end{bmatrix}$
is a linear combination of $X_1=\begin{bmatrix}2\\-1\\1\end{bmatrix}$
and $X_2=\begin{bmatrix}3\\3\\2\end{bmatrix}$.

<font color='Green'><b>Solution</b></font>:
Since $V$ is a linear combinations of $X_1$ and $X_2$, there exist $a$
and $b$ such that

\begin{align*}
V&=aX_1+bX_2,
\\
\begin{bmatrix}1\\r\\0\end{bmatrix}&=a\begin{bmatrix}2\\-1\\1\end{bmatrix}+b\begin{bmatrix}3\\3\\2\end{bmatrix},
\\
\begin{bmatrix}1\\r\\0\end{bmatrix}&=\begin{bmatrix}2a\\-a\\a\end{bmatrix}+\begin{bmatrix}3b\\3b\\2b\end{bmatrix}\end{align*}

However, the last equation is equivalent to

$$\begin{cases}
2a+3b=1\\
-a+3b=r\\
a+2b=0.
\end{cases}$$

The corresponding augmented matrix is

$$\label{Ex1.16.eq.01}
\left[\begin{array}{cc|c} 2 & 3 & 1\\ -1 & 3 & r\\ 1 & 2 & 0 \end{array}\right]$$

REF:

\begin{align*}
\left[\begin{array}{cc|c} 2 & 3 & 1\\ -1 & 3 & r\\ 1 & 2 & 0 \end{array}\right]
&\Rightarrow{R_{1} \leftrightarrow R_{3}} \Rightarrow
\left[\begin{array}{cc|c} 1 & 2 & 0\\ -1 & 3 & r\\ 2 & 3 & 1 \end{array}\right]
\\ &
\Rightarrow -2R_{1}+R_{3}\rightarrow R_{3}, {R_{1}+R_{2}\rightarrow R_{2}} \Rightarrow
\left[\begin{array}{cc|c} 1 & 2 & 0\\ 0 & 5 & r\\ 0 & -1 & 1 \end{array}\right]
\\ &
\Rightarrow{R_{2} \leftrightarrow R_{3}} \Rightarrow
\left[\begin{array}{cc|c} 1 & 2 & 0\\ 0 & -1 & 1\\ 0 & 5 & r \end{array}\right]
\\ &
\Rightarrow{-R_{2}\rightarrow R_{2}} \Rightarrow
\left[\begin{array}{cc|c} 1 & 2 & 0\\ 0 & 1 & -1\\ 0 & 5 & r \end{array}\right]
\\ &
\Rightarrow{-5R_{2}+R_{3}\rightarrow R_{3}} \Rightarrow
\left[\begin{array}{cc|c} {1} & 2 & 0\\ 0 & {1} & -1\\ 0 & 0 & r+5 \end{array}\right]\end{align*}

Note that the linear system is inconsistent if $r+5\neq 0$, and the linear system is consistent
if $r+5= 0$. Therefore, since we are looking for a solution for this
system, only  $r = -5$ is acceptable.

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***