# Multiplication of Matrices

`````{admonition} Row and Column Vectors
:class: tip

**Column Matrices (Vectors):**
Column matrices, also known as column vectors, are matrices of size $n \times 1$. In other words, they have $n$ rows and only one column. Similarly, row matrices of size $1 \times n$ are also referred to as row vectors. Vectors are essential objects in linear algebra and have various applications in mathematics, physics, computer science, and engineering.

For a column matrix $A$ of size $n \times 1$:
\begin{align*} A = \begin{bmatrix}
a_{1} \\
a_{2} \\
\vdots \\
a_{n}
\end{bmatrix} \end{align*}

- Each entry $a_i$ in the column matrix $A$ represents the element in the $i^{th}$ row of the matrix.



**Row Matrices (Row Vectors):**
For a row matrix $B$ of size $1 \times n$:
\begin{align*} B = \begin{bmatrix}
b_{1} & b_{2} & \dots & b_{n}
\end{bmatrix} \end{align*}

- Each entry $b_i$ in the row matrix $B$ represents the element in the $i^{th}$ column of the matrix.

`````

<font color='Blue'><b>Example</b></font>: For example, if $A$ is a column matrix of size $3 \times 1$, it would look like this:
\begin{align*} A = \begin{bmatrix}
a_{1} \\
a_{2} \\
a_{3}
\end{bmatrix} \end{align*}


Likewise, if $B$ is a row matrix of size $1 \times 4$, it would look like this:
\begin{align*} B = \begin{bmatrix}
b_{1} & b_{2} & b_{3} & b_{4}
\end{bmatrix} \end{align*}

Both column matrices (vectors) and row matrices (row vectors) play a crucial role in linear algebra, and they are used to represent quantities such as position, velocity, and forces in physics, as well as data in various applications like machine learning and statistics.


Before we explain multiplying matrices. Let's explain the multiplication of a row vector by a column vector. For row vector $X$ and a column vector $Y$. we have,

\begin{align*}
\begin{bmatrix}    x_1 & x_2 & \dots & x_n \end{bmatrix}
\begin{bmatrix}    y_1\\ y_2 \\ \vdots \\ y_n \\  \end{bmatrix}=
x_1y_1+x_2y_2+\ldots+x_ny_n=\sum_{j=1}^{n}x_jy_j.\end{align*}


For a row vector $X$ and a column vector $Y$, where both have the same size $n \times 1$, we perform the multiplication as follows:

\begin{align*} X = \begin{bmatrix} x_1 & x_2 & \dots & x_n \end{bmatrix} \end{align*}

\begin{align*} Y = \begin{bmatrix} y_1 \\ y_2 \\ \vdots \\ y_n \end{bmatrix} \end{align*}

The multiplication of the row vector $X$ and column vector $Y$ is given by the sum of the products of their corresponding entries:

\begin{align*} \begin{bmatrix} x_1 & x_2 & \dots & x_n \end{bmatrix} \begin{bmatrix} y_1 \\ y_2 \\ \vdots \\ y_n \end{bmatrix} = x_1y_1 + x_2y_2 + \ldots + x_ny_n \end{align*}

This can be represented using summation notation as:

\begin{align*} \begin{bmatrix} x_1 & x_2 & \dots & x_n \end{bmatrix} \begin{bmatrix} y_1 \\ y_2 \\ \vdots \\ y_n \end{bmatrix} = \sum_{j=1}^{n} x_j y_j \end{align*}

Where:
- $x_j$ represents the $j$-th entry in the row vector $X$.
- $y_j$ represents the $j$-th entry in the column vector $Y$.
- The summation symbol $\sum$ denotes the sum of the products of the corresponding entries, ranging from $j=1$ to $j=n$.

In other words, we multiply each entry in the row vector $X$ by the corresponding entry in the column vector $Y$, and then sum up these products to get the final result.

<font color='Blue'><b>Example</b></font>: For example, if we have:

\begin{align*} X = \begin{bmatrix} 2 & 3 & 4 \end{bmatrix} \end{align*}

\begin{align*} Y = \begin{bmatrix} 1 \\ -1 \\ 2 \end{bmatrix} \end{align*}

The multiplication of the row vector $X$ and column vector $Y$ is:

\begin{align*} \begin{bmatrix} 2 & 3 & 4 \end{bmatrix} \begin{bmatrix} 1 \\ -1 \\ 2 \end{bmatrix} = (2 \cdot 1) + (3 \cdot (-1)) + (4 \cdot 2) = 2 - 3 + 8 = 7 \end{align*}

***

<font color='Blue'><b>Example</b></font>: Evaluate $\begin{bmatrix}    1 & 2 & 3  \end{bmatrix}\begin{bmatrix}    -2 \\ 1 \\ 4  \end{bmatrix}$.

<font color='Green'><b>Solution</b></font>:

We have the row vector:
\begin{align*} X = \begin{bmatrix} 1 & 2 & 3 \end{bmatrix} \end{align*}

And the column vector:
\begin{align*} Y = \begin{bmatrix} -2 \\ 1 \\ 4 \end{bmatrix} \end{align*}

To multiply the row vector $X$ by the column vector $Y$, we follow these steps:

1. Take the first entry of the row vector ($1$) and the first entry of the column vector ($-2$), then multiply them together: $(1) \times (-2) = -2$.
2. Take the second entry of the row vector ($2$) and the second entry of the column vector ($1$), then multiply them together: $(2) \times (1) = 2$.
3. Take the third entry of the row vector ($3$) and the third entry of the column vector ($4$), then multiply them together: $(3) \times (4) = 12$.

Finally, add up the results of these individual multiplications:

\begin{align*} (-2) + 2 + 12 = 12 \end{align*}

So, the result of multiplying the row vector $X$ and the column vector $Y$ is $12$.

In summary, the multiplication of a row vector by a column vector is obtained by taking the dot product of the vectors. It involves multiplying each corresponding pair of entries and then summing up these products. The dot product is a common operation in linear algebra and has various applications in vector calculations and geometry.

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
    
In general, matrix multiplication is not commutative! (i.e, $AB\neq BA)$. However, there are some examples where $AB=BA$.
    
</div>

<font color='Blue'><b>Example</b></font>: Let $A=\begin{bmatrix} 2 & 0 \\  0 & 2 \end{bmatrix}$ and $B=\begin{bmatrix} 1 & 2 \\  3 & 4 \end{bmatrix}$. Then

$$
AB=\begin{bmatrix} 2 & 4 \\  6& 8 \end{bmatrix} \text{ and } BA=\begin{bmatrix} 2 & 4 \\  6& 8 \end{bmatrix}.
$$

Note that usually $AB$ is different from $BA$.

***
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***