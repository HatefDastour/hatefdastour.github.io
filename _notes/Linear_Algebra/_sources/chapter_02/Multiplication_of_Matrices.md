# 2.1.3 Multiplication of Matrices

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Row and Column Vectors
</b></font>

Column matrices (matrices of size $n\times 1$ or $1\times n$) are called vectors. If $X$ is such a matrix, 
* If $A = \begin{bmatrix}a_{1} \\a_{2} \\ \vdots\\ a_{n}\end{bmatrix}$ (a column matrix), $a_i$ denotes the entry of $A$ in the $i^{th}$ row.
* If $B = \begin{bmatrix}b_{1} & b_{2} & \dots & b_{n}\end{bmatrix}$ ( a row matrix), $b_i$ denotes the entry of $B$ in the $i^{th}$ column.
</div>
****:

Before we explain multiplying matrices. Let's explain the multiplication of a row vector by a column vector. For row vector $X$ and a column vector $Y$. we have,

\begin{align*}
\begin{bmatrix}    x_1 & x_2 & \dots & x_n \end{bmatrix}
\begin{bmatrix}    y_1\\ y_2 \\ \vdots \\ y_n \\  \end{bmatrix}=
x_1y_1+x_2y_2+\ldots+x_ny_n=\sum_{j=1}^{n}x_jy_j.\end{align*}

<font color='Blue'><b>Example</b></font>: Evaluate $\begin{bmatrix}    1 & 2 & 3  \end{bmatrix}\begin{bmatrix}    -2 \\ 1 \\ 4  \end{bmatrix}$.

<font color='Green'><b>Solution</b></font>:

\begin{align*}
\begin{bmatrix}    {1} & {2} & {3}  \end{bmatrix}\begin{bmatrix}    {-2} \\ {1} \\ {4}  \end{bmatrix}
=(1)(-2)+(2)(1)+(3)(4)=-2+2+12=12.\end{align*}
***

<div class="alert alert-warning" role="alert">
<font size="+1"><b>
Remark:
</b></font>

For matrices $A$ and $B$, to form the product $AB$, the number of columns of $A$ must be **equal** to the number of rows of $B$. 

Consider a product $AB$ where $A$ has size $m\times n$ and $B$ has size $n\times  p$. Then, the product in terms of size of matrices is given by
\begin{align*}
(m\times \overbrace{n) (n}^{\text{these must match!}} \times  p ) = m\times  p
\end{align*}
</div>

We explain this using an example:

<font color='Blue'><b>Example</b></font>: Let $A=\begin{bmatrix}3 & -1 \\ 0 & 2\end{bmatrix}$ and $B=\begin{bmatrix}2 & 4 \\ 1 & 7\end{bmatrix}$.  Evaluate $AB$.

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
