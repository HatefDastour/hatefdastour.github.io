# Matrix Arithmetic

**Matrix**: A rectangular array of numbers is called a matrix (the
plural is matrices), and the numbers are called the entries of the
matrix. Matrices are usually denoted by uppercase letters: $A$, $B$,
$C$, ....

For example,

\begin{align*}
A=\begin{bmatrix} 1 & 0 \\ 2 & 1\end{bmatrix}_{2\times 2},~B=\begin{bmatrix} 1 & 3 & \frac{3}{2}\\ 2 & 1 & \sqrt{5}\end{bmatrix}_{2\times 3}
,~C=\begin{bmatrix} 1\\ 2 \\ -1 \end{bmatrix}_{3\times 1}\end{align*}

are matrices.

-   A matrix with $m$ rows and $n$ columns is referred to as an
    $m\times n$ matrix or as having size $m\times n$. For example,
    matrices $A$, $B$, and $C$ above have sizes $2\times 2$,
    $2\times 3$, and $3\times 1$, respectively.

-   $A$ matrix of size $1\times n$ is called a **row matrix** (it just
    has a row), whereas one of size $m\times1$ is called a **column
    matrix** (it has only a column). For example, matrix $C$ above is an
    example of a column matrix.

Each entry of a matrix is identified by the row and column in which it
lies. The rows are numbered from the top down, and the columns are
numbered from left to right. Then the **$(i,~j)$-entry** of a matrix is
the number lying simultaneously in row $i$ and column $j$.

For example, consider
$D=\begin{bmatrix} 5 & 3 & 1\\ 0 & 2 & -1\end{bmatrix}$.

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

**square matrix**: Matrices of size $n\times n$ for some $n$ are called **square
matrices**.

Examples of square matrices:

\begin{align*}
\begin{bmatrix} 1 & 0 \\ 2 & 1\end{bmatrix},\quad
\begin{bmatrix} 1 & 0 & 1\\ 2 & 1 & -1 \\ 3 & \sqrt{5} & \frac{5}{2}\end{bmatrix},\quad
\begin{bmatrix} 17 & 24 & 1 & 8 & 15\\ 23 & 5 & 7 & 14 & 16\\ 4 & 6 & 13 & 20 & 22\\ 10 & 12 & 19 & 21 & 3\\ 11 & 18 & 25 & 2 & 9\end{bmatrix}
\end{align*}

**zero matrix**
The $m\times n$ zero matrix is the $m\times n$ matrix having every entry equal to zero. It is denoted by $O_{m,n}$ (or simply just 0).


Examples of zero matrices:
\begin{align*}
O_{2\times 2}=\begin{bmatrix} 0 & 0\\ 0 & 0\end{bmatrix},\quad
O_{2\times 3}=\begin{bmatrix} 0 & 0 & 0\\ 0 & 0 & 0\end{bmatrix},\quad
O_{3\times 1}=\begin{bmatrix} 0\\ 0\\ 0  \end{bmatrix}
\end{align*}

Two matrices $A$ and $B$ are called **equal** (written $A = B$) if and
only if:

1.  They have the same size.

2.  Corresponding entries are equal.

For instance,

\begin{align*}
\begin{bmatrix}  0 & 0 \\   0 & 0 \end{bmatrix} \neq \begin{bmatrix}  0 & 0 \\  0 & 0 \\  0 & 0 \end{bmatrix},
\quad
\begin{bmatrix}  1 & 2 \\   3 & 4 \end{bmatrix} \neq \begin{bmatrix}  2 & 1 \\  4 & 3 \end{bmatrix},
\quad
\begin{bmatrix}  1 & 2 \\   3 & 4 \end{bmatrix} = \begin{bmatrix}  1 & 2 \\  3 & 4 \end{bmatrix}.\end{align*}

Addition of Matrices
-------------------------------------

We can add two matrices only if all matrices in the sum need have the same size.

**Matrix Addition**: If $A$ and $B$ are matrices of the same size, their sum $A+B$ is the matrix formed by adding corresponding entries.

<font color='Blue'><b>Example</b></font>:
Let $A=\begin{bmatrix}  1 & -2 & 4\\ 3 & 0 & 7 \end{bmatrix}$
and $B=\begin{bmatrix}  6 & 2 & 4\\ -2 & 1 & -1 \end{bmatrix}$. Find $A+B$.
***
<font color='Green'><b>Solution</b></font>:

\begin{align*}
A+B &=\begin{bmatrix}  1 & -2 & 4\\ 3 & 0 & 7 \end{bmatrix}+\begin{bmatrix}  6 & 2 & 4\\ -2 & 1 & -1 \end{bmatrix}
\\ &
=\begin{bmatrix}  1+6 & -2+2 & 4+4\\ 3+(-2) & 0+1 & 7+(-1) \end{bmatrix}=\begin{bmatrix}  7 & 0 & 8\\ 1 & 1 & 6 \end{bmatrix}.
\end{align*}
***

<font color='Blue'><b>Example</b></font>:
If $C=\begin{bmatrix}  1 & -3 & 4\\ 0 & 1 & 2 \end{bmatrix}$
and $D=\begin{bmatrix}  1 & 1\\ 1 & 3 \end{bmatrix}$, we cannot have $C+D$ since $C$ is $2\times 3$ and $D$ is $2\times 2$.

<div class="alert alert-block alert-info">
<font size="+1"><b>
Proposition - Properties of Matrix Addition:
</b></font>
    
<p>Let <span class="math inline">\(A\)</span>,<span class="math inline">\(B\)</span> and <span class="math inline">\(C\)</span> be matrices. Then, the following properties hold.</p>
<ul>
<li><p>Commutative Law of Addition: <span class="math display">\[\begin{aligned}
 A+B = B+A \end{aligned}\]</span></p></li>
<li><p>Associative Law of Addition: <span class="math display">\[\begin{aligned}
 (A+B)+C = A+(B+C) \end{aligned}\]</span></p></li>
<li><p>Existence of an Additive Identity: There exists a zero matrix 0 such that <span class="math display">\[\begin{aligned}
 A+0 = A \end{aligned}\]</span></p></li>
<li><p>Existence of an Additive Inverse: There exists a matrix <span class="math inline">\(-A\)</span> such that <span class="math display">\[\begin{aligned}
 A+(-A) = 0 \end{aligned}\]</span></p></li>
</ul>
    
</div>

Scalar Multiplication of Matrices
--------------------------

**Scalar Multiplication of Matrices**: If $A =\left[a_{i,j}\right]$ and $k$ is a scalar, then
$kA = \left[k~a_{i,j}\right]$.

<font color='Blue'><b>Example</b></font>: If $A=\begin{bmatrix}1 & 2 \\ 3 & 4\end{bmatrix}$, find $cA$ and $-A$.
***
<font color='Green'><b>Solution</b></font>:

\begin{align*}
3A&=\begin{bmatrix}1 & 2 \\ 3 & 4\end{bmatrix}=\begin{bmatrix}(3)(1) & (3)(2) \\ (3)(3) & (3)(4)\end{bmatrix}
=\begin{bmatrix}3 & 6\\ 9 & 12\end{bmatrix},\\
-A&=\begin{bmatrix}1 & 2 \\ 3 & 4\end{bmatrix}=\begin{bmatrix}(-1)(1) & (-1)(2) \\ (-1)(3) & (-1)(4)\end{bmatrix}
=\begin{bmatrix}-1 & -2\\ -3 & -4\end{bmatrix}.\end{align*}
***

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
Substraction is similar to addition since $A-B=A+(-B)$. However, substraction is not commutative which means for arbitrary matrices $A$ and $B$
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

Multiplication of Matrices
--------------------------------

**Row and Column Vectors**:
Matrices of size $n\times 1$ or $1\times n$ are called vectors. If $X$
is such a matrix, then we write $x_i$ to denote the entry of $X$ in the
$i^{th}$ row of a column matrix, or the $i^{th}$ column of a row matrix.
The $n\times 1$ matrix

\begin{align*}
X=\begin{bmatrix}    x_1\\ \vdots \\ x_n \\  \end{bmatrix}\end{align*}

is called a **column vector** (column matrix). The $1\times n$ matrix

\begin{align*}
X=\begin{bmatrix}    x_1 & \dots & x_n \end{bmatrix}\end{align*}

is
called a **row vector** (row matrix).

Before we explain multiplying matrices. Let's explain the multiplication of a row vector by a column vector. For row vector $X$ and a column vector $Y$. we have,

\begin{align*}
\begin{bmatrix}    x_1 & x_2 & \dots & x_n \end{bmatrix}
\begin{bmatrix}    y_1\\ y_2 \\ \vdots \\ y_n \\  \end{bmatrix}=
x_1y_1+x_2y_2+\ldots+x_ny_n=\sum_{j=1}^{n}x_jy_j.\end{align*}

<font color='Blue'><b>Example</b></font>: Evaluate $\begin{bmatrix}    1 & 2 & 3  \end{bmatrix}\begin{bmatrix}    -2 \\ 1 \\ 4  \end{bmatrix}$.
***
<font color='Green'><b>Solution</b></font>:

\begin{align*}
\begin{bmatrix}    {1} & {2} & {3}  \end{bmatrix}\begin{bmatrix}    {-2} \\ {1} \\ {4}  \end{bmatrix}
=(1)(-2)+(2)(1)+(3)(4)=-2+2+12=12.\end{align*}
***

For matrices $A$ and $B$, in order to form the product $AB$, the number of columns of $A$ must equal the number of rows of $B$. Consider a product $AB$ where $A$ has size $m\times n$ and $B$ has size $n\times  p$. Then, the product in terms of size of matrices is given by
\begin{align*}
(m\times \overbrace{n) (n}^{\text{these must match!}} \times  p ) = m\times  p
\end{align*}

We explain this using an example:

<font color='Blue'><b>Example</b></font>: Let $A=\begin{bmatrix}3 & -1 \\ 0 & 2\end{bmatrix}$ and $B=\begin{bmatrix}2 & 4 \\ 1 & 7\end{bmatrix}$.  Evaluate $AB$.
***
<font color='Green'><b>Solution</b></font>:
$A$ is a $2\times 2$ matrix, and $B$ is a $2\times 2$ matrix. Therefore,
$AB$ is $2\times 2$ matrix as well. Evaluating each entry of $AB$:

-   **$(1,~1)$-entry** of a matrix $AB$: We multiply row $1$ of matrix
    $A$ and column $1$ of matrix $B$ (It is similar to multiplying a row
    vector by a column vector).
    
    \begin{align*}
    \left[\begin{array}{cc}3 & -1\\ 0 & 2\end{array}\right]
    \left[\begin{array}{>{\columncolor{blue!10}}cc}2 & 4 \\ 1 & 7\end{array}\right]\end{align*}
    
    \begin{align*}
    \text{$(1,~1)$-entry of a matrix $AB$}=\begin{bmatrix}3 & -1\end{bmatrix}\begin{bmatrix}2 & 1\end{bmatrix}=(3)(2)+(-1)(1)=3+2=5.\end{align*}

-   **$(1,~2)$-entry** of a matrix $AB$: We multiply row $1$ of matrix
    $A$ and column $2$ of matrix $B$.
    
    \begin{align*}
    \left[\begin{array}{cc}3 & -1\\0 & 2\end{array}\right]
    \left[\begin{array}{c>{\columncolor{blue!10}}c}2 & 4 \\ 1 & 7\end{array}\right]\end{align*}
    
    \begin{align*}
    \text{$(1,~2)$-entry of a matrix $AB$}=\begin{bmatrix}3 & -1\end{bmatrix}\begin{bmatrix}4 & 7\end{bmatrix}=(3)(4)+(-1)(7)=12-7=5.\end{align*}

-   **$(2,~1)$-entry** of a matrix $AB$: We multiply row $2$ of matrix
    $A$ and column $1$ of matrix $B$.
    
    \begin{align*}
    \left[\begin{array}{cc}3 & -1\\  0 & 2\end{array}\right]
    \left[\begin{array}{>{\columncolor{blue!10}}cc}2 & 4 \\ 1 & 7\end{array}\right]\end{align*}
    
    \begin{align*}
    \text{$(2,~1)$-entry of a matrix $AB$}=\begin{bmatrix}0 & 2\end{bmatrix}\begin{bmatrix}2 & 1\end{bmatrix}=(0)(2)+(2)(1)=0+2=2.\end{align*}

-   **$(2,~2)$-entry** of a matrix $AB$: We multiply row $2$ of matrix
    $A$ and column $2$ of matrix $B$.
    
    \begin{align*}
    \left[\begin{array}{cc}3 & -1\\  0 & 2\end{array}\right]
    \left[\begin{array}{c>{\columncolor{blue!10}}c}2 & 4 \\ 1 & 7\end{array}\right]\end{align*}
    
    \begin{align*}
    \text{$(2,~1)$-entry of a matrix $AB$}=\begin{bmatrix}0 & 2\end{bmatrix}\begin{bmatrix}1 & 7\end{bmatrix}=(0)(1)+(2)(7)=0+14=14.\end{align*}

Therefore, $AB=\begin{bmatrix}5 & 5\\ 2 & 14\end{bmatrix}$.
***

<font color='Blue'><b>Example</b></font>: Compute $AB$ where $A=\begin{bmatrix}1 & 2 \\ -3 & 0 \\ 1 & -4 \end{bmatrix}$ and
 $B=\begin{bmatrix}  1 & -1 & 2 \\ 3 & -2 & 1 \end{bmatrix}$.
***
<font color='Green'><b>Solution</b></font>:
$A$ is a $3\times 2$ matrix, and $B$ is a $2\times 3$ matrix. Therefore,
$AB$ is $3\times 3$ matrix.\
Evaluating the first row of $AB$:

\begin{align*}
\left[\begin{array}{cc}1 & 2 \\ -3 & 0 \\ 1 & -4 \end{array}\right]
\left[\begin{array}{>{\columncolor{blue!15}}c>{\columncolor{yellow!30}}c>{\columncolor{cyan!20}}c}
1 & -1 & 2 \\ 3 & -2 & 1  \end{array}\right]
&=
\begin{bmatrix}  (1)(1)+(2)(3) & (1)(-1)+(2)(-2) & (1)(2)+(2)(1)\\ \centerdot & \centerdot & \centerdot \\ \centerdot & \centerdot & \centerdot\end{bmatrix} \\
&=
\left[\begin{array}{ccc}   7 & -5 & 4\\ \centerdot & \centerdot & \centerdot \\ \centerdot & \centerdot & \centerdot \end{array}\right]\end{align*}

Evaluating the second row of $AB$:

\begin{align*}
\left[\begin{array}{cc}1 & 2 \\  -3 & 0 \\ 1 & -4 \end{array}\right]
\left[\begin{array}{>{\columncolor{blue!15}}c>{\columncolor{yellow!30}}c>{\columncolor{cyan!20}}c}
1 & -1 & 2 \\ 3 & -2 & 1  \end{array}\right]
&=
\begin{bmatrix}  7 & -5 & 4\\ (-3)(1)+(0)(3) & (-3)(-1)+(0)(-2) & (-3)(2)+(0)(1) \\ \centerdot & \centerdot & \centerdot\end{bmatrix}
\\
&=
\left[\begin{array}{ccc}  7 & -5 & 4\\  -3 & 3 & -6 \\ \centerdot & \centerdot & \centerdot \end{array}\right]\end{align*}

Evaluating the third row of $AB$:

\begin{align*}
\left[\begin{array}{cc}1 & 2 \\  -3 & 0 \\  1 & -4 \end{array}\right]
\left[\begin{array}{>{\columncolor{blue!15}}c>{\columncolor{yellow!30}}c>{\columncolor{cyan!20}}c}
1 & -1 & 2 \\ 3 & -2 & 1  \end{array}\right]
&=
\begin{bmatrix}  7 & -5 & 4\\ -3 & 3 & -6  \\ (1)(1)+(-4)(3) & (1)(-1)+(-4)(-2) & (1)(2)+(-4)(1) \end{bmatrix}
\\
&=
\left[\begin{array}{ccc}  7 & -5 & 4\\  -3 & 3 & -6 \\  -11 & 7 & -2 \end{array}\right]\end{align*}

Therefore,
$AB=\begin{bmatrix} 7 & -5 & 4\\ -3 & 3 & -6\\ -11 & 7 & -2 \end{bmatrix}$.
***

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
In general, matrix multiplication is not commutative! (i.e, $AB\neq BA)$. However, there are some examples where $AB=BA$ and in this case we say $A$ and $B$ commute.
    
</div>

<font color='Blue'><b>Example</b></font>: Let $A=\begin{bmatrix} 2 & 0 \\  0 & 2 \end{bmatrix}$ and $B=\begin{bmatrix} 1 & 2 \\  3 & 4 \end{bmatrix}$. Then

$$
AB=\begin{bmatrix} 2 & 4 \\  6& 8 \end{bmatrix} \text{ and } BA=\begin{bmatrix} 2 & 4 \\  6& 8 \end{bmatrix}.
$$

Note that usually $AB$ is different from $BA$.
