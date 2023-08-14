# Matrix Arithmetic


`````{admonition} Matrix
:class: tip

A matrix is a two-dimensional array of numbers, symbols, or expressions arranged in rows and columns. Each element within the matrix is referred to as an entry. Matrices are commonly represented using uppercase letters such as $A$, $B$, $C$, and so on. The dimensions of a matrix are determined by the number of rows and columns it contains. For example, if a matrix has $m$ rows and $n$ columns, it is said to be an "$m \times n$ matrix.

A general representation of a matrix can be expressed as:
\begin{align*}
\begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\ a_{21} & a_{22} & \dots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m1} & a_{m2} & \dots & a_{mn} 
\end{bmatrix}
\end{align*}
Where each $a_{ij}$ denotes the entry at the $i$-th row and $j$-th column of the matrix $A$. Matrices are fundamental objects in linear algebra and are used in various mathematical and scientific applications, such as solving systems of linear equations, transformations in computer graphics, optimization problems, and much more.

`````

<font color='Blue'><b>Example</b></font>: $A$, $B$, and $C$ are matrices.
\begin{align*}
A=\begin{bmatrix} 1 & 0 \\ 2 & 1\end{bmatrix}_{2\times 2},~B=\begin{bmatrix} 1 & 3 & \frac{3}{2}\\ 2 & 1 & \sqrt{5}\end{bmatrix}_{2\times 3}
,~C=\begin{bmatrix} 1\\ 2 \\ -1 \end{bmatrix}_{3\times 1}
\end{align*}


`````{admonition} Remark
:class: important

* **Row Matrix**: A row matrix is a matrix of size $1 \times n$, meaning it has only one row and $n$ columns. It is also commonly known as a row vector. A row matrix can be represented as:
\begin{align*}
\begin{bmatrix}
r_{1} & r_{2} & \dots & r_{n}
\end{bmatrix},
\end{align*}
where $r_{i}$ denotes the entry at the $i$-th column of the row matrix $R$.

* **Column Matrix**: A column matrix is a matrix of size $n \times 1$, meaning it has only one column and $n$ rows. It is also known as a column vector. A column matrix can be represented as:
\begin{align*}
\begin{bmatrix}
c_{1} \\
c_{2} \\
\vdots \\
c_{n}
\end{bmatrix},
\end{align*}
where $c_{i}$ denotes the entry at the $i$-th row of the column matrix $C$.

`````

<font color='Blue'><b>Example</b></font>: Matrices $A$, $B$, and $C$ above have sizes $2\times 2$, $2\times 3$, and $3\times 1$, respectively. Also, the matrix $C$ above is an example of a column matrix.

`````{admonition} Remark
:class: important


In a matrix, the arrangement of elements is such that the rows are numbered from top to bottom, and the columns are numbered from left to right. Therefore, the $(i,~j)$-entry of a matrix refers to the number located at the intersection of the $i$-th row and the $j$-th column.

For example, consider the following matrix:

\begin{align*}
A = \begin{bmatrix}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{bmatrix}
\end{align*}

In this matrix, the $(2,~3)$-entry, denoted as $a_{23}$, is the element located in the second row (row 2) and the third column (column 3). Similarly, the $(1,~2)$-entry, denoted as $a_{12}$, is the element located in the first row (row 1) and the second column (column 2).

The notation $(i,~j)$-entry is a convenient way to describe and access individual elements within a matrix, making it clear which specific row and column an element belongs to. It is widely used in linear algebra and various other mathematical fields that involve working with matrices.

`````

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


In a matrix $A$, the entry at the $i$-th row and $j$-th column is denoted by $a_{ij}$. Matrix $A$ itself is displayed as follows:

\begin{align*}
A =
\begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
a_{21} & a_{22} & \dots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn}
\end{bmatrix}
= \left[ a_{ij} \right]
\end{align*}

In this representation, $A$ is a matrix with $m$ rows and $n$ columns. The elements $a_{ij}$ within the matrix are the individual entries, where $i$ denotes the row number and $j$ denotes the column number. The notation $\left[ a_{ij} \right]$ is a concise way of expressing the collection of entries in matrix $A$.

For instance, let's consider a specific example:

\begin{align*}
A =
\begin{bmatrix}
2 & 4 & 6 \\
1 & 3 & 5 \\
\end{bmatrix}
= \left[ a_{ij} \right]
\end{align*}

In this case, we have a $2 \times 3$ matrix $A$ with the entries $a_{11} = 2$, $a_{12} = 4$, $a_{13} = 6$, $a_{21} = 1$, $a_{22} = 3$, and $a_{23} = 5$. The notation $\left[ a_{ij} \right]$ serves as a compact representation of the entire matrix.


`````{admonition} Square Matrix
:class: tip


A matrix is called a **square matrix** if it has the same number of rows and columns. In other words, for a square matrix, the number of rows is equal to the number of columns.
`````

<font color='Blue'><b>Example</b></font>: For example:

\begin{align*}
A = \begin{bmatrix}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{bmatrix}
\end{align*}

The matrix $A$ above is square because it has 3 rows and 3 columns.

Square matrices are of particular interest in various mathematical applications, including linear algebra and geometry. They have unique properties and can be subject to special operations that do not apply to non-square matrices. For instance, square matrices are necessary for finding determinants, eigenvalues, and eigenvectors, which play essential roles in many mathematical and scientific disciplines.

<font color='Blue'><b>Example</b></font>: square matrices:

\begin{align*}
\begin{bmatrix} 1 & 0 \\ 2 & 1\end{bmatrix},\quad
\begin{bmatrix} 1 & 0 & 1\\ 2 & 1 & -1 \\ 3 & \sqrt{5} & \frac{5}{2}\end{bmatrix},\quad
\begin{bmatrix} 17 & 24 & 1 & 8 & 15\\ 23 & 5 & 7 & 14 & 16\\ 4 & 6 & 13 & 20 & 22\\ 10 & 12 & 19 & 21 & 3\\ 11 & 18 & 25 & 2 & 9\end{bmatrix}
\end{align*}

`````{admonition} Zero Matrix
:class: tip

A matrix with all its entries set to zero is called a **zero matrix**. If a zero matrix has a size of $m\times n$, it is denoted as $O_{m,n}$ or simply just 0.

The zero matrix $O_{m,n}$ of size $m\times n$ is represented as:

\begin{align*} O_{m,n} = \begin{bmatrix}
0 & 0 & \dots & 0 \\
0 & 0 & \dots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \dots & 0
\end{bmatrix} \end{align*}

In this matrix, all entries are zeros, and it has $m$ rows and $n$ columns.

`````


<font color='Blue'><b>Example</b></font>: For example:

\begin{align*} O_{3,4} = \begin{bmatrix}
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0
\end{bmatrix} \end{align*}

Here, we have a zero matrix of size $3\times 4$.

The zero matrix is a fundamental concept in linear algebra and is often used as a neutral element in various matrix operations. It has specific properties that make it essential in understanding and solving systems of linear equations, performing matrix addition, and exploring transformations in linear algebra.

Some other zero matrices:
\begin{align*}
O_{2\times 2}=\begin{bmatrix} 0 & 0\\ 0 & 0\end{bmatrix},\quad
O_{2\times 3}=\begin{bmatrix} 0 & 0 & 0\\ 0 & 0 & 0\end{bmatrix},\quad
O_{3\times 1}=\begin{bmatrix} 0\\ 0\\ 0  \end{bmatrix}
\end{align*}

`````{admonition} Equal Matrices
:class: tip

Two matrices $A$ and $B$ are considered **equal** (written as $A = B$) if and only if the following two conditions are satisfied:

1. They have the same size: Matrices $A$ and $B$ must have the same number of rows and columns. In other words, they should be of the same dimension. If $A$ is an $m\times n$ matrix, then $B$ must also be an $m\times n$ matrix for them to be equal.

2. Corresponding entries are equal: For each pair of entries in the same position (row $i$ and column $j$) of matrices $A$ and $B$, the values must be equal. Mathematically, this can be expressed as $a_{ij} = b_{ij}$ for all $i$ and $j$, where $a_{ij}$ and $b_{ij}$ are the entries at position $(i,j)$ in matrices $A$ and $B$, respectively.

In summary, two matrices are considered equal if they have the same size (same number of rows and columns) and if all corresponding entries in the matrices are equal.

`````

<font color='Blue'><b>Example</b></font>:

For example:

\begin{align*} A = \begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix} \end{align*}

\begin{align*} B = \begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix} \end{align*}

In this case, $A$ and $B$ are equal since they have the same size (both are $2\times 2$ matrices), and all corresponding entries are the same ($a_{ij} = b_{ij}$ for all $i$ and $j$). Therefore, we can say $A = B$ for this example.


<font color='Blue'><b>Example</b></font>:

1. **$\begin{bmatrix} 0 & 0 \\ 0 & 0 \end{bmatrix} \neq \begin{bmatrix} 0 & 0 \\ 0 & 0 \\ 0 & 0 \end{bmatrix}$**:
   The first comparison is between two matrices with different sizes. The first matrix on the left is a $2\times 2$ matrix (2 rows and 2 columns), while the matrix on the right is a $3\times 2$ matrix (3 rows and 2 columns). Since the matrices have different dimensions, they cannot be equal.

2. **$\begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} \neq \begin{bmatrix} 2 & 1 \\ 4 & 3 \end{bmatrix}$**:
   The second comparison is between two different $2\times 2$ matrices. While both matrices have the same size (both are $2\times 2$), the corresponding entries in the matrices are different. For example, in the first matrix, the entry in the first row and the second column is 2, while in the second matrix, it is 1. Since there is at least one entry that differs between the two matrices, they are not equal.

3. **$\begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}$**:
   The third comparison is between two identical $2\times 2$ matrices. Both matrices have the same size, and all corresponding entries are the same. For example, in both matrices, the entry in the first row and the second column is 2. Since all entries are equal between the two matrices, they are indeed equal.
