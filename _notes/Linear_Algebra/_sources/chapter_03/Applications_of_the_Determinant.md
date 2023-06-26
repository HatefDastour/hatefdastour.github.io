# Applications of the Determinant

## A Formula for the Inverse

<div class="alert alert-info" role="alert">
<font size="+1"><b>
The Cofactor Matrix
</b></font>

The cofactor matrix of an $n\times n$ matrix $A$ can be defined as follows,
\begin{align*}
cof (A) =\begin{bmatrix}
           cof (A)_{11} & cof (A)_{12} & \dots & cof (A)_{1n}\\
           cof (A)_{21} & cof (A)_{22} & \dots & cof (A)_{2n}\\
           \vdots & \vdots & \dots & \vdots\\
           cof (A)_{n1} & cof (A)_{n2} & \dots & cof (A)_{nn}\\
         \end{bmatrix}
\end{align*}
where $cof (A)_{ij}$ is the $ij^{\text{th}}$ cofactor of matrix $A$.
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
The Adjugate Matrix
</b></font>

The transpose of the cofactor matrix $A$, i.e. $cof (A)^T$, is called the adjugate of matrix $A$. We have,
\begin{align*}
adj (A) =\left[cof (A)_{ji}\right]=\begin{bmatrix}
           cof (A)_{11} & cof (A)_{21} & \dots & cof (A)_{n1}\\
           cof (A)_{12} & cof (A)_{22} & \dots & cof (A)_{n2}\\
           \vdots & \vdots & \dots & \vdots\\
           cof (A)_{1n} & cof (A)_{2n} & \dots & cof (A)_{nn}\\
         \end{bmatrix}
\end{align*}
The adjugate of matrix $A$ is also known as the adjoint of $A$.
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark
</b></font>
    
The adjugate of $A$ is also called the classical adjoint of $A$ and denoted by $adj(A)$; however, the term “adjoint” has another meaning in mathematics.
</div>

<font color='Blue'><b>Example</b></font>:
Find $adj(A)$ if $A=\begin{bmatrix} 4 & 0 & 3 \\ 1 & 9 & 7 \\ 0 & 6 & 4 \end{bmatrix}$.

<font color='Green'><b>Solution</b></font>:
First we need to find $minor(A)_{11}$, $minor(A)_{12}$, $minor(A)_{13},\ldots,~ minor(A)_{33}$. We have
\begin{align*}
cof (A) =\begin{bmatrix}
           {\color{red}+}minor(A)_{11} & {\color{red}-}minor(A)_{12} & {\color{red}+}minor(A)_{13}\\
           {\color{red}-}minor(A)_{21} & {\color{red}+}minor(A)_{22} & {\color{red}-}minor(A)_{23}\\
           {\color{red}+}minor(A)_{31} & {\color{red}-}minor(A)_{32} & {\color{red}+}minor(A)_{33}\\
         \end{bmatrix}
\end{align*}
where
\begin{align*}
&minor(A)_{11}=\left[\begin{array}{ccc}4 & 0 & 3 \\ 1 & 9 & 7 \\ 0 & 6 & 4  \end{array}\right]=-6,
&minor(A)_{12}=\left[\begin{array}{ccc}4 & 0 & 3 \\ 1 & 9 & 7 \\ 0 & 6 & 4  \end{array}\right]=4,
\\
&minor(A)_{13}=\left[\begin{array}{ccc}4 & 0 & 3 \\ 1 & 9 & 7 \\ 0 & 6 & 4  \end{array}\right]=6,
&minor(A)_{21}=\left[\begin{array}{ccc}4 & 0 & 3\\ 1 & 9 & 7 \\ 0 & 6 & 4  \end{array}\right]=-18,
\\
&minor(A)_{22}=\left[\begin{array}{ccc}4 & 0 & 3\\  1 & 9 & 7 \\ 0 & 6 & 4  \end{array}\right]=16,
&minor(A)_{23}=\left[\begin{array}{ccc}4 & 0 & 3\\ 1 & 9 & 7 \\ 0 & 6 & 4  \end{array}\right]=24,
\\
&minor(A)_{31}=\left[\begin{array}{ccc}4 & 0 & 3 \\ 1 & 9 & 7 \\ 0 & 6 & 4  \end{array}\right]=-27,
&minor(A)_{32}=\left[\begin{array}{ccc}4 & 0 & 3\\  4 & 5 & 6 \\ 0 & 6 & 4  \end{array}\right]=25,
\\
&minor(A)_{33}=\left[\begin{array}{ccc}4 & 0 & 3 \\ 1 & 9 & 7 \\ 0 & 6 & 4  \end{array}\right]
=36.&
\end{align*}
Therefore,
\begin{equation*}
cof (A) =\begin{bmatrix}-6 & -4 & 6\\ 18 & 16 & -24\\ -27 & -25 & 36\end{bmatrix},
\end{equation*}
and
\begin{equation*}
adj(A)=\left(cof (A)\right)^T =\begin{bmatrix}-6 & 18 & -27\\ -4 & 16 & -25\\ 6 & -24 & 36\end{bmatrix},
\end{equation*}
***

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: The Inverse and the Determinant
</b></font>
    
Let $A$ be an $n\times n$ matrix. Then 
\begin{align*}
A\,adj (A) = adj (A)\,A = \det(A)I
\end{align*}
Moreover, $A$ is invertible if and only if $\det(A) \neq 0$. In this case we have:
\begin{align*}
A^{-1}  = \frac{1}{\det(A)} adj(A).
\end{align*}
</div>

In particular, for a invertible $2\times 2$ matrix $A=\begin{bmatrix}a & b \\ c & d\end{bmatrix}$, we have
\begin{align*}
adj(A)=\begin{bmatrix}d & -b \\ -c & a\end{bmatrix}\quad \text{and} \quad A^{-1}  = \frac{1}{\det(A)} adj(A)=\frac{1}{ad-bc}\begin{bmatrix}d & -b \\ -c & a\end{bmatrix}.
\end{align*}

<font color='Blue'><b>Example</b></font>:
Find the inverse of $A=\begin{bmatrix}1 & 2\\ 3 & 4\end{bmatrix}$.

<font color='Green'><b>Solution</b></font>:
\begin{align*}
A^{-1}  = \frac{1}{(1)(4)-(2)(3)}\begin{bmatrix}4 & -2\\ -3 & 1\end{bmatrix}=
-\frac{1}{2}\begin{bmatrix}4 & -2\\ -3 & 1\end{bmatrix}
=\begin{bmatrix}-2 & 1\\ \frac{3}{2} & -\frac{1}{2}\end{bmatrix}.
\end{align*}

***

<font color='Blue'><b>Example</b></font>:
Find $A$ if $(3I-A^T)^{-1}=2\begin{bmatrix} 1 & 1\\ 2 & 3  \end{bmatrix}$.

<font color='Green'><b>Solution</b></font>:

We know that for an invertible matrix $X$, $\left(X^{-1}\right)^{-1}=X$. Therefore,
$$\left(\left(3I-A^T\right)^{-1}\right)^{-1}=\left(2\begin{bmatrix}1 & 1\\ 2 & 3\end{bmatrix}\right)^{-1}.$$
Now since, for an invertible matrix $X$, $\left(cX\right)^{-1}=\dfrac{1}{c}X^{-1}$,
$$3I-A^T=\frac{1}{2}\left(\begin{bmatrix}1 & 1\\ 2 & 3\end{bmatrix}\right)^{-1}.$$
Moreover, it can be easily seen that,
\begin{align*}
\left(\begin{bmatrix}1 & 1\\ 2 & 3\end{bmatrix}\right)^{-1}=
\frac{1}{(1)(3)-(1)(2)} \begin{bmatrix}3 & -1\\ -2 & 1\end{bmatrix}=
\frac{1}{1} \begin{bmatrix}3 & -1\\ -2 & 1\end{bmatrix}=
\begin{bmatrix}3 & -1\\ -2 & 1\end{bmatrix}.
\end{align*}
It follows that,
\begin{align*}
& 3I-A^T=\frac{1}{2}\begin{bmatrix}3 & -1\\ -2 & 1\end{bmatrix},\\
\text{Subtracting }3I\text{ from both sides} \Rightarrow \quad &
{3I}-A^T-{3I}=\frac{1}{2}\begin{bmatrix}3 & -1\\ -2 & 1 \end{bmatrix}-3I,\\
\Rightarrow\quad &
-A^T=\begin{bmatrix}\frac{3}{2} & -\frac{1}{2}\\ -1 & \frac{1}{2}\end{bmatrix}-\begin{bmatrix} 3 & 0\\ 0 & 3 \end{bmatrix}
=\begin{bmatrix}-\frac{3}{2} & -\frac{1}{2}\\ -1 & -\frac{5}{2} \end{bmatrix},
\\
{\text{Multiplying both sides by }-1}\Rightarrow \quad & A^{T}=\begin{bmatrix}\frac{3}{2} & \frac{1}{2}\\ 1 & \frac{5}{2} \end{bmatrix}
\\
\Rightarrow \quad &
A=(A^T)^T=\begin{bmatrix}\frac{3}{2} & 1\\ \frac{1}{2} & \frac{5}{2}\end{bmatrix}=
\frac{1}{2}\begin{bmatrix}3 & 2\\ 1 & 5\end{bmatrix}.
\end{align*}

***

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Proposition
</b></font>

If A is $n\times n$, $n \geq 2$, then
\begin{align*}
\det(adj(A))=(\det(A))^{n-1}.
\end{align*}
    
</div>

**Proof**: Since $A$ is invertible, $\det(A) \neq 0$. In this case we have:
\begin{align*}
A^{-1}   & = \frac{1}{\det(A)} adj(A)\\
{\text{Multiplying both sides by }\det(A)} \quad  & \Rightarrow\det(A).A^{-1}  = adj(A)
\end{align*}
\begin{align*}
\det(adj(A))&= \det\left(\underbrace{\det(A)}_{\text{Just a scalar}}.\underbrace{A^{-1}}_{n\times n\text{ matrix}}\right)
\\
&= \left(\det(A)\right)^{n} \det\left(A^{-1}\right)
\\
&= \left(\det(A)\right)^{n} \frac{1}{\det\left(A\right)}
\\
&= \left(\det(A)\right)^{n-1}.
\end{align*}

<font color='Blue'><b>Example</b></font>:
Suppose $A$ is a $2\times 2$ and invertible matrix. Find $\det\left(2\,A(adj(A))^{-1}\right)$.

<font color='Green'><b>Solution</b></font>:

\begin{align*}
\det\left(2\,A(adj(A))^{-1}\right)&=2^2\det(A)\det\left(\left(adj(A)\right)^{-1}\right)
\\
&=4\det(A)\frac{1}{\det\left(adj(A)\right)}.
\end{align*}
Here $n=2$
\begin{align*}
\det(adj(A))=(\det(A))^{2-1}=\det(A)
\end{align*}
Therefore,
\begin{align*}
\det\left(2\,A(adj(A))^{-1}\right)&=4\,{\det(A)}\frac{1}{{\det(A)}}=4.
\end{align*}

***

<font color='Blue'><b>Example</b></font>:
Let $A$ be a $2\times 2$ matrix. The reduced row-echelon form of $A$ is
the identity matrix, and is obtained by performing the following two
elementary row operations in order:

1.  First multiply row 2 by 2.

2.  Then add $-1$ times row 2 to row 1.

Find Matrix $A$.

<font color='Green'><b>Solution</b></font>:

We need to use the form $B =UA$ with $B=I_2$. We have $I=UA=(E_2E_1)A$,
where

1.  First multiply row 2 by 2:
    $E_2=E(2,2)=\begin{bmatrix} 1 & 0 \\ 0 & 2 \end{bmatrix}$.

2.  Then add $-1$ times row 2 to row 1:
    $E_2=E((-1)\times \, 2+ \, 1)=\begin{bmatrix} 1 & -1\\ 0 & 1 \end{bmatrix}$.

Therefore,

\begin{align*}
A=&U^{-1}=(E_{1}E_{2})^{-1}=E_{1}^{-1}E_{2}^{-1}=
\begin{bmatrix} 1 & 0 \\ 0 & 2 \end{bmatrix}^{-1}
\begin{bmatrix} 1 & -1\\ 0 & 1 \end{bmatrix}^{-1}\\ &
=\left(\frac{1}{2}\begin{bmatrix} 2 & 0 \\ 0 & 1 \end{bmatrix}\right)
\left(\frac{1}{1}\begin{bmatrix} 1 & 1\\ 0 & 1 \end{bmatrix}\right)=
\left[\begin{array}{cc} 1 & 0\\ 0 & \frac{1}{2} \end{array}\right]
\left[\begin{array}{cc} 1 & 1\\ 0 & 1 \end{array}\right]
=\left[\begin{array}{cc} 1 & 1\\ 0 & \frac{1}{2} \end{array}\right].\end{align*}

***

## Cramer’s Rule

<div class="alert alert-info" role="alert">
<font size="+1"><b>
The Vector Form of a System of Linear Equations
</b></font>

Consider the following system of linear equations
\begin{align*}
\begin{cases}
a_{11}x_1+\ldots+a_{1n}x_{n}=b_1\\
a_{21}x_1+\ldots+a_{2n}x_{n}=b_2\\
\vdots \\
a_{m1}x_1+\ldots+a_{mn}x_{n}=b_m\\
\end{cases}
\end{align*}
We can express this system of linear equations in **vector form** as follows:
\begin{align*}
x_1\begin{bmatrix}a_{11}\\a_{21}\\ \vdots \\ a_{m1}\end{bmatrix}+
x_2\begin{bmatrix}a_{12}\\a_{22}\\ \vdots \\ a_{m2}\end{bmatrix}+
\ldots+
x_n\begin{bmatrix}a_{1n}\\a_{2n}\\ \vdots \\ a_{mn}\end{bmatrix}=
\begin{bmatrix}b_{1}\\b_{2}\\ \vdots \\ b_{m}\end{bmatrix}
\end{align*}
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
The Matrix Form of a System of Linear Equations
</b></font>

Consider the following system of linear equations
\begin{align*}
\begin{cases}
a_{11}x_1+\ldots+a_{1n}x_{n}=b_1\\
a_{21}x_1+\ldots+a_{2n}x_{n}=b_2\\
\vdots \\
a_{m1}x_1+\ldots+a_{mn}x_{n}=b_m.
\end{cases}
\end{align*}
We also can express this system in **matrix form** as follows.
\begin{align*}
\begin{bmatrix}a_{11} & a_{12} & \dots & a_{1n}\\a_{21} & a_{22} & \dots & a_{2n}\\
\vdots & \vdots & \ddots & \vdots \\a_{m1} & a_{m2} & \dots & a_{mn}\\ \end{bmatrix}
\begin{bmatrix}x_{1}\\x_{2}\\ \vdots \\ x_{n}\end{bmatrix}=
\begin{bmatrix}b_{1}\\b_{2}\\ \vdots \\ b_{m}\end{bmatrix}
\end{align*}
</div>

Typically, the matrix form of a system of linear equations is shown with $AX = B$ where $A$ is a $m \times n$ matrix, $X$ is a $n \times 1$ matrix. and $B$ is a $m \times 1$ matrix.

<font color='Blue'><b>Example</b></font>:
Convert the following system into $AX=B$ form.
\begin{align*}
\begin{cases}
3x_1-2x_2+7x_3=4,\\
5x_1+3x_2-x_3=0.
\end{cases}
\end{align*}

<font color='Green'><b>Solution</b></font>:

\begin{align*}
\begin{bmatrix} 3 & -2 & 7\\ 5 & 3 & -1 \end{bmatrix}
\begin{bmatrix} x_1\\x_2\\x_3 \end{bmatrix}=
\begin{bmatrix} 4\\0 \end{bmatrix}
\end{align*}

***

For a system of equations given by $AX = B$, and we can find its solutions $X$ using $A^{-1}$ (if $A^{-1}$ exists),

\begin{align*}
AX &= B\\
A^{-1}(AX) &= A^{-1} B\\
(A^{-1}A) X &= A^{-1}B\\
IX &= A^{-1} B\\
X &= A^{-1}B
\end{align*}
Observe that the solutions $X$ to the system are given by $X =A^{-1} B$. Since we assumed that $A^{-1}$ exists, we can use
the formula for $A^{-1}$ given above. Substituting this formula into the equation for $X$, we have
\begin{align*}
X = A^{-1} B = \frac{1}{\det(A)}  adj(A)B
\end{align*}

<font color='Blue'><b>Example</b></font>:
Solve the following system using matrix inverses.
\begin{align*}
\begin{cases}
x_1+2x_2=3\\
2x_1+3x_2=4.
\end{cases}
\end{align*}

<font color='Green'><b>Solution</b></font>:
Matrix form:
\begin{align*}
\underbrace{\begin{bmatrix} 1 & 2\\ 2 & 3 \end{bmatrix}}_{{\color{red}A}}
\underbrace{\begin{bmatrix} x_1\\x_2\end{bmatrix}}_{{\color{red}X}}
=\underbrace{\begin{bmatrix} 3\\4 \end{bmatrix}}_{{\color{red}B}}
\end{align*}
$A=\begin{bmatrix} 1 & 2\\ 2 & 3 \end{bmatrix}$ is invertible since $\det(A)=-1\neq0$. Therefore,
\begin{align*}
X &= A^{-1}B=\begin{bmatrix} 1 & 2\\ 2 & 3 \end{bmatrix}^{-1}\begin{bmatrix} 3\\4 \end{bmatrix}
=\frac{1}{(1)(3)-(2)(2)}\begin{bmatrix} 3 & -2\\ -2 & 1 \end{bmatrix}\begin{bmatrix} 3\\4 \end{bmatrix}
\\&
=\frac{1}{(-1)}\begin{bmatrix} 3 & -2\\ -2 & 1 \end{bmatrix}\begin{bmatrix} 3\\4 \end{bmatrix}
=-\begin{bmatrix} 1\\-2 \end{bmatrix}= \begin{bmatrix} -1\\ 2\end{bmatrix}.
\end{align*}

***

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark
</b></font>
    
Generally, it is customary to use $\begin{bmatrix}x_1 & x_2 & \dots & x_n \end{bmatrix}^{T}$ instead of $\begin{bmatrix}x_1 \\ x_2 \\ \vdots \\ x_n. \end{bmatrix}$.
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Cramer’s rule
</b></font>

Let $A$ be an $n\times  n$ invertible matrix. To solve the system $AX = B$ for $X=\begin{bmatrix}x_1 & x_2 & \dots & x_n \end{bmatrix}^{T}$, Cramer’s rule can be used:
\begin{align*}
x_i =\frac{\det(A_i )}{\det(A)}
\end{align*}
where $A_i$ is the matrix obtained by replacing the $i^{\text{th}}$ column of $A$ with the column matrix
\begin{align*}
B=\begin{bmatrix}b_1 \\ b_2 \\ \vdots \\ b_n \end{bmatrix}.
\end{align*}
</div>

<font color='Blue'><b>Example</b></font>:
Use Cramer’s rule to find the solution to
\begin{align*}
\begin{cases}
x+2y+z = 1,\\
2x-y-z = 2,\\
x+z = 1.
\end{cases}
\end{align*}

<font color='Green'><b>Solution</b></font>:
We can express this system in matrix form as follows
\begin{align*}
\underbrace{\begin{bmatrix}1 & 2 & 1\\ 2 & -1 & -1 \\ 1 & 0 & 1\end{bmatrix}}_{A}
\underbrace{\begin{bmatrix}x \\ y \\ z\end{bmatrix}}_{X}=
\underbrace{\begin{bmatrix}1 \\ 2 \\ 1 \end{bmatrix}}_{B}
\end{align*}
Here $\left|\begin{array}{ccc} 1 & 2 & 1\\ 2 & -1 & -1\\ 1 & 0 & 1 \end{array}\right|=-6\neq0$. Therefore, we can use the Cramer's rule.

Finding $x$: we replace the 1st column of $A$ with $B$ and get $A_1$. Then, form $x =\dfrac{\det(A_1)}{\det(A)}$.
\begin{align*}
A_1=\left[\begin{array}{>{\columncolor{green!30}}ccc} 1 & 2 & 1\\ 2 & -1 & -1\\ 1 & 0 & 1\end{array} \right]
\end{align*}
and
\begin{align*}
x =\frac{\det(A_1)}{\det(A)}=\frac{\left|\begin{array}{ccc}1 & 2 & 1\\ 2 & -1 & -1 \\ 1 & 0 & 1\end{array}\right|}{\left|\begin{array}{ccc}1 & 2 & 1\\ 2 & -1 & -1 \\ 1 & 0 & 1 \end{array}\right|}=1.
\end{align*}
Finding $y$: we replace the 2nd column of $A$ with $B$ and get $A_2$. Then, form $y =\dfrac{\det(A_2)}{\det(A)}$.

\begin{align*}
A_2=\left[\begin{array}{c>{\columncolor{green!30}}cc} 1 & 1 & 1\\ 2 & 2 & -1 \\ 1 & 1 & 1\end{array} \right]
\Rightarrow \qquad
y =\frac{\det(A_2)}{\det(A)}=\frac{\left|\begin{array}{ccc}1 & 1 & 1\\ 2 & 2 & -1 \\ 1 & 1 & 1\end{array}\right|}{\left|\begin{array}{ccc}1 & 2 & 1\\ 2 & -1 & -1 \\ 1 & 0 & 1 \end{array}\right|}=0.
\end{align*}
Moreover, $z$ can be calculated as follows.
\begin{align*}
A_3=\left[\begin{array}{cc>{\columncolor{green!30}}c} 1 & 2 & 1\\ 2 & -1 & 2 \\ 1 & 0 & 1 \end{array} \right]
\Rightarrow \qquad
z =\frac{\det(A_3)}{\det(A)}=\frac{\left|\begin{array}{ccc}1 & 2 & 1\\ 2 & -1 & 2 \\ 1 & 0 & 1 \end{array}\right|}
{\left|\begin{array}{ccc}1 & 2 & 1\\ 2 & -1 & -1 \\ 1 & 0 & 1 \end{array}\right|}=0.
\end{align*}

***

## Polynomial Interpolation

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Polynomial and the Degree of the Polynomial
</b></font>

An expression of the form $a_nx^n+a_{n-1}x^{n-1}+a_{n-2}x^{n-2}+\ldots+a_{1}x^{1}+a_0$ is called a **polynomial**. In this expression
$a_{0},~a_{1},~\ldots,~a_{n}$ are numbers and $x$ is a variable. If the coeficient of $x^n$ is nonzero ($a_n \neq 0$), the integer
$n$ is called the **degree of the polynomial**, and $a_n$ is called the leading coefficient.
</div>

|                             |                                                              |
|-----------------------------|--------------------------------------------------------------|
|  A polynomial of degree $1$ |                            $ax+b$                            |
| A polynomial of degree  $2$ |                          $ax^2+bx+c$                         |
| A polynomial of degree  $3$ |                       $ax^3+bx^2+cx+d$                       |
|           $\vdots$          |                           $\vdots$                           |
|  A polynomial of degree $n$ | $a_nx^n+a_{n-1}x^{n-1}+a_{n-2}x^{n-2}+\ldots+a_{1}x^{1}+a_0$ |


<div class="alert alert-info" role="alert">
<font size="+1"><b>
Interpolating Polynomial
</b></font>

Assume that $n$ data pairs $(x_1,y_1 )$, $(x_2 , y_2 )$, ..., $(x_n , y_n )$ are available in a way that the $x_i$ are distinct. Then, there exists a unique polynomial
\begin{equation*}
p(x) = r_0 +r_1 x+r_2 x^2 +\ldots+r_{n-1} x^{n-1}
\end{equation*}
such that $p(x_i ) = y_i$ for each $i = 1, 2, \ldots, n$.

For this data, this polynomial is called the **interpolating polynomial**.
</div>

<div class="alert alert-success" role="alert">

The procedure to find $p(x)$ for given $x_1 , x_2 , \ldots, x_n$ and their corresponding $y_1 , y_2 , \ldots, y_n$:

1.  Assume that desired polynomial $p(x)$ is given by $p(x) = r_0 +r_1 x+r_2 x^2 +\ldots+r_{n-1} x^{n-1}$.

2.  $p(x_i ) = y_i$ for all $i = 1, 2, \ldots, n$ so that
    \begin{align*}
	\begin{cases}
    r_0 +r_1 x_{1}+r_2 x_{1}^2 +\ldots+r_{n-1} x_{1}^{n-1}=y_{1}\\
    r_0 +r_1 x_{2}+r_2 x_{2}^2 +\ldots+r_{n-1} x_{2}^{n-1}=y_{2}\\    \ldots \\
    r_0 +r_1 x_{n}+r_2 x_{n}^2 +\ldots+r_{n-1} x_{n}^{n-1}=y_{n}
    \end{cases}
	\end{align*}
    
    In matrix form:
	
    \begin{align*}
	\begin{bmatrix}
    1 & x_{1} & x_{1}^{2} & \dots & x_{1}^{n}\\
    1 & x_{2} & x_{2}^{2} & \dots & x_{2}^{n}\\
    \vdots & \vdots & \vdots & & \vdots \\
    1 & x_{n} & x_{n}^{2} & \dots & x_{n}^{n}\\
    \end{bmatrix}
    \begin{bmatrix}r_{1}\\r_{2}\\ \vdots \\ r_{n-1}
	\end{bmatrix}    =
    \begin{bmatrix}y_{1}\\y_{2}\\ \vdots \\ y_{m}
	\end{bmatrix}.
	\end{align*}

3.  The augmented matrix of this system of equations:
\begin{align*}
\left[\begin{array}{ccccc|c}
1 & x_{1} & x_{1}^{2} & \dots & x_{1}^{n} & y_{1}\\
1 & x_{2} & x_{2}^{2} & \dots & x_{2}^{n} & y_{2}\\
\vdots & \vdots & \vdots & & \vdots  & \vdots \\
1 & x_{n} & x_{n}^{2} & \dots & x_{n}^{n} &  y_{m}\\
\end{array}\right]
\end{align*}

4.  By solving this system of equations, we get a  **unique** solution $r_0$ ,
    $r_1$, ..., $r_{n-1}$ . Using these values, we can construct $p(x)$ , and estimate the value of $p(a)$ for any $x = a$.
</div>

<font color='Blue'><b>Example</b></font>:
Consider the data points $(-2,1)$, $(0,1)$, $(2,9)$, $(3,16)$ . Find an interpolating polynomial $p(x)$ of degree at most three, and estimate the value of $p(1)$.

<font color='Green'><b>Solution</b></font>:
We like to identify 
\begin{equation*}
p(x) = r_0 +r_1 x+r_2 x^2 +r_{3} x^{3}
\end{equation*}
in a way that $p(-2)=1$, $p(0)=1$, $p(2)=9$ and $p(3)=16$.

We can substitute the known values in for $x$ and solve for $r_0$, $r_1$, $r_2$ and $r_3$. Using the given points, the system of equations is
\begin{align*}
&p(-2)=1 &\Rightarrow& & r_{0}-2\,r_{1}+4\,r_{2}-8\,r_{3}=1&\\
&p(0)=1 & \Rightarrow& & r_{0}=1&\\
&p(2)=9 & \Rightarrow& & r_{0}+2\,r_{1}+4\,r_{2}+8\,r_{3}=9&\\
&p(3)=16 & \Rightarrow& & r_{0}+3\,r_{1}+9\,r_{2}+27\,r_{3}=16&
\end{align*}
The augmented matrix:
\begin{equation*}
\left[\begin{array}{cccc|c}
1 & -2 & 4 & -8 & 1\\ 1 & 0 & 0 & 0 & 1\\ 1 & 2 & 4 & 8 & 9\\ 1 & 3 & 9 & 27 & 16
\end{array}\right]
\end{equation*}
In RREF:
\begin{equation*}
\left[\begin{array}{cccc|c}
1 & 0 & 0 & 0 & 1\\ 0 & 1 & 0 & 0 & 2\\ 0 & 0 & 1 & 0 & 1\\ 0 & 0 & 0 & 1 & 0
\end{array}\right]
\end{equation*}
Therefore, $r_0 = 1$, $r_1 = 2$ , $r_2 = 1$, $r_3 = 0$ and $p(x) = x^2+2\,x+1$ . To estimate the value of $p(1)$, we compute
\begin{equation*}
p(1) = (1)^2+2(1)+1= 4.
\end{equation*}

<center>
<iframe src="https://www.desmos.com/calculator/tpnftqinpd?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>
</center>

***
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***