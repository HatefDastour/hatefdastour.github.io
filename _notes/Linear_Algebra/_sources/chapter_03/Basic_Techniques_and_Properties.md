# Basic Techniques and Properties

## Cofactors and Determinants

**Determinant**: The determinant of an $n\times n$ matrix $A$, denoted by $\det(A)$ or $|A|$, is a very important number associated with $A$.

If $A$ is a $2\times 2$ matrix, the determinant is given by the following formula.

**Determinant of a Two By Two Matrix**: Let $A=\begin{bmatrix}a & b \\ c & d\end{bmatrix}$. Then
\begin{equation*}
\det(A)=\left|\begin{array}{cc} a & b \\ c & d \end{array}\right|= ad-cb
\end{equation*}

<font color='Blue'><b>Example</b></font>:
Find $det(A)$ for the matrix $A = \begin{bmatrix}1 & 2\\ 5 & 1\end{bmatrix}$.

<font color='Green'><b>Solution</b></font>: $\det(A)=(1)(1)-(2)(5)=1-10=-9.$

***

**The $ij^{\text{th}}$  Minor of a Matrix**: Let $A$ be a $3\times 3$ matrix. The $ij^{\text{th}}$ minor of $A$ , denoted as $minor(A)_{ij}$, is the determinant of the $2\times 2$ matrix which results from deleting the $i^{\text{th}}$ row and the $j^{\text{th}}$ column of $A$.

In general, if $A$ is an $n\times n$ matrix, then the $ij^{\text{th}}$  minor of $A$ is the determinant of \linebreak the $(n-1)\times(n-1)$ matrix which results from deleting the $i^{\text{th}}$ row and the $j^{\text{th}}$ column of $A$.

<font color='Blue'><b>Example</b></font>:
If $A = \begin{bmatrix}1 & 2 & 3\\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{bmatrix}$, find $minor(A)_{11}$, $minor(A)_{12}$, $minor(A)_{13}$, $minor(A)_{21},~\ldots$.

<font color='Green'><b>Solution</b></font>:

\begin{align*}
minor(A)_{11}&=
\left|\begin{array}{cc} 5 & 6\\ 8 & 9 \end{array}\right|=(5)(9)-(6)(8)=-3.
\\
minor(A)_{12}&=
\left|\begin{array}{cc} 4 & 6\\ 7 & 9 \end{array}\right|=(4)(9)-(6)(7)=-6.
\\
minor(A)_{13}&=
\left|\begin{array}{cc} 4 & 5\\ 7 & 8 \end{array}\right|=-3.
\end{align*}

\begin{align*}
minor(A)_{21}&=
\left|\begin{array}{cc} 2 & 3\\ 8 & 9 \end{array}\right|=-6.
\\
minor(A)_{22}&=
\left|\begin{array}{cc} 1 & 3\\ 7 & 9 \end{array}\right|=-12.
\\
minor(A)_{23}&=
\left|\begin{array}{cc} 1 & 2\\ 7 & 8\end{array}\right|=-6.
\end{align*}

\begin{align*}
minor(A)_{31}&=
\left|\begin{array}{cc} 2 & 3\\ 5 & 6 \end{array}\right|=-3.
\\
minor(A)_{32}&=
\left|\begin{array}{cc} 1 & 3\\ 4 & 6 \end{array}\right|=-6.
\\
minor(A)_{33}&=
\left|\begin{array}{cc} 1 & 2\\ 4 & 5\end{array}\right|=-3.
\end{align*}

***

**The $ij^{\text{th}}$  Cofactor of a Matrix**: Suppose $A$ is an $n\times n$ matrix. The $ij^{\text{th}}$ \textbf{cofactor}, denoted by $cof (A)_{ij}$ is defined to be
$$cof (A) _{ij} = (-1)^{i+j} minor(A)_{ij}$$

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark
</b></font>
    
<ul>
<li><p>We use cofactors to compute the determinant of a matrix.</p></li>
<li><p><span class="math inline">\(cof (A) _{ij}\)</span> provides the sign of (<span class="math inline">\(i\)</span>,<span class="math inline">\(j\)</span>)-entry of <span class="math inline">\(A\)</span> multiplied by <span class="math inline">\(minor(A)_{ij}\)</span>.</p></li>
<li><p>Sign patterns: <span class="math display">\[\begin{aligned}
\left[\begin{array}{cc} {\color{blue}+} & {\color{red}-} \\ {\color{red}-} & {\color{blue}+} \end{array}\right],~
\left[\begin{array}{ccc}
{\color{blue}+} & {\color{red}-} &  {\color{blue}+} \\
{\color{red}-} & {\color{blue}+} & {\color{red}-} \\
{\color{blue}+} & {\color{red}-} &  {\color{blue}+}
\end{array}\right]
,~
\left[\begin{array}{cccc}
{\color{blue}+} & {\color{red}-} &  {\color{blue}+} & {\color{red}-}\\
{\color{red}-} & {\color{blue}+} & {\color{red}-} & {\color{blue}+} \\
{\color{blue}+} & {\color{red}-} &  {\color{blue}+} & {\color{red}-} \\
{\color{red}-} & {\color{blue}+} & {\color{red}-} & {\color{blue}+} \\
\end{array}\right],\ldots\end{aligned}\]</span></p></li>
</ul>
</div>

**The Determinant of a Three By Three Matrix**: Let $A$ be a $3\times 3$ matrix. Then, $\det(A)$ is calculated by picking a row (or column) and taking the product of each entry in that row (column) with its cofactor and adding these products together. This process when applied to the $i^{\text{th}}$ row (column) is known as expanding along the $i^{\text{th}}$ row (column) as is given by

\begin{equation*}
det(A) = a_{i1}\, cof (A)_{i1} +a_{i2}\, cof (A)_{i2} +a_{i3}\, cof (A)_{i3}
\end{equation*}

<font color='Blue'><b>Example</b></font>:
Evaluate $\det(A)$ if $A=\begin{bmatrix} 1 & 8 & 2 \\ 0 & -1 & 1 \\ 1 & 0 & 3 \end{bmatrix}$.

<font color='Green'><b>Solution</b></font>:
Let's expand along row 1.

\begin{align*}
A=\left[\begin{array}{ccc} 1 & 8 & 2 \\ 0 & -1 & 1 \\ 1 & 0 & 3 \end{array}\right]
\quad \text{Sign pattern}= \left[\begin{array}{ccc}  + & - &  + \\ - & + &  - \\ + & - &  + \\ \end{array}\right]
\end{align*}

\begin{align*}
\left|\begin{array}{ccc} 1 & 8 & 2\\ 0 & -1 & 1\\ 1 & 0 & 3 \end{array}\right|
&= a_{11}\, cof (A)_{11} +a_{12}\, cof (A)_{12} +a_{13}\, cof (A)_{13}
\\ &
= a_{11}\, \underbrace{(1)minor(A)_{11}}_{cof (A)_{11}} +a_{12}\, \underbrace{(-1)minor(A)_{12}}_{cof (A)_{12}} +a_{13}\,\underbrace{(1)minor(A)_{13}}_{cof (A)_{13}}\\ &=
(1)\left|\begin{array}{ccc} 1 & 8 & 2 \\ 0 & -1 & 1 \\ 1 & 0 & 3  \end{array}\right|
-(8) \left|\begin{array}{ccc} 1 & 8 & 2 \\ 0 & -1 & 1 \\ 1 & 0 & 3  \end{array}\right|
+(3)\left|\begin{array}{ccc}1 & 2 & 3\\ 4 & 5 & 6 \\ 7 & 8 & 9  \end{array}\right|
\\ &
=\left|\begin{array}{cc} -1 & 1\\ 0 & 3 \end{array}\right|
-8\left|\begin{array}{cc} 0 & 1\\ 1 & 3 \end{array}\right|
+2\left|\begin{array}{cc} 0 & -1\\ 1 & 0 \end{array}\right|
\\ &
=-3-(8)(-1)+(2)(1)=7.
\end{align*}
***

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: The Determinant is Well Defined
</b></font>
    
<p>Expanding the <span class="math inline">\(n\times n\)</span> matrix along any row or column always gives the <u>same answer</u>, which is the determinant.</p>

</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark
</b></font>
    
<p>Generally, we usually pick a row or column with <strong>most number of zeros</strong> for evaluating the determinan of a matrix.</p>

</div>

<font color='Blue'><b>Example</b></font>:
Let $A=\begin{bmatrix} 0 & 0 & 1 & 2 \\ 1 & 0 & 0 & 1 \\ 2 & 0 & -1 & 2 \\ 3 & 2 & 0 & 0 \end{bmatrix}$. Evaluate $\det(A)$.

<font color='Green'><b>Solution</b></font>:
Let's expand along the second column.

\begin{align*}
A=\left[\begin{array}{c>{\columncolor{green!20}}ccc} 0 & 0 & 1 & 2 \\ 1 & 0 & 0 & 1 \\ 2 & 0 & -1 & 2 \\ 3 & 2 & 0 & 0 \end{array}\right]
\quad \text{Sign pattern}=
\left[\begin{array}{c>{\columncolor{green!20}}ccc} + & - &  + & - \\ - & + & - &  + \\ + & - &  + & -  \\  - & + & - &  + \end{array}\right]
\end{align*}

\begin{align*}
\det(A)&=\left|\begin{array}{cccc} 0 & 0 & 1 & 2 \\ 1 & 0 & 0 & 1 \\ 2 & 0 & -1 & 2 \\ 3 & 2 & 0 & 0 \end{array}\right|
= a_{12}\, cof (A)_{12} +a_{22}\, cof (A)_{22} +a_{32}\, cof (A)_{32}+a_{42}\, cof (A)_{42}
\\ &
= -a_{12}\, minor(A)_{12} +a_{22}\, minor(A)_{22} -a_{32}\,minor(A)_{32}+a_{42}\,minor(A)_{42}
\\ &
= +a_{42}\,minor(A)_{42}
\\ &
=a_{42}\,minor(A)_{42}=2
\left|\begin{array}{cccc} 0 & 0 & 1 & 2 \\ 1 & 0 & 0 & 1 \\ 2 & 0 & -1 & 2 \\ 3 & 2 & 0 & 0  \end{array}\right|
=2\left|\begin{array}{ccc} 0 & 1 & 2 \\ 1 & 0 & 1 \\ 2 & -1 & 2\end{array}\right|
\end{align*}

Now we need to evaluate the determinant of $\begin{bmatrix}0 & 1 & 2 \\ 1 & 0 & 1 \\ 2 & -1 & 2\end{bmatrix}$. The first row (with one zero) or the second column (with one zero) are good choices. Let's expand along the first row.

\begin{align*}
A=\left[\begin{array}{ccc} 0 & 1 & 2 \\ 1 & 0 & 1 \\ 2 & -1 & 2 \end{array}\right]
\quad \text{Sign pattern}= \left[\begin{array}{ccc}  + & - &  + \\ - & + &  - \\ + & - &  + \\ \end{array}\right]
\end{align*}

Therefore,

\begin{align*}
\det(A)&=2\left|\begin{array}{ccc} 0 & 1 & 2 \\ 1 & 0 & 1 \\ 2 & -1 & 2\end{array}\right|
\\ & = 2\left(
(0)\left|\begin{array}{ccc} 0 & 1 & 2 \\ 1 & 0 & 1 \\ 2 & -1 & 2  \end{array}\right|
-(1) \left|\begin{array}{ccc} 0 & 1 & 2 \\ 1 & 0 & 1 \\ 2 & -1 & 2  \end{array}\right|
+(2)\left|\begin{array}{ccc} 0 & 1 & 2 \\ 1 & 0 & 1 \\ 2 & -1 & 2  \end{array}\right|\right)
\\ &
= 2\left(
(0)\left|\begin{array}{cc} 0 & 1\\ -1 & 2 \end{array}\right|
-(1)\left|\begin{array}{cc} 1 & 1\\ 2 & 2 \end{array}\right|
+(2)\left|\begin{array}{cc} 1 & 0\\ 2 & -1 \end{array}\right|\right)
\\ &
=2\left((0)(1)-(1)(0)+(2)(-1) \right)=(2)(-2)=-4.
\end{align*}
***

## The Determinant of a Triangular Matrix

**Triangular Matrices**: A triangular matrix is a matrix that is either an upper triangular
matrix or a lower triangular matrix.

-   An **upper triangular matrix** is defined as a matrix for which all
    entries **below** the main diagonal are equal to zero.
    
	\begin{align*}
    \begin{bmatrix}  * & * & \dots & * \\   0 & * & \dots & \vdots \\   \vdots & \vdots & \ddots & * \\   0 & \dots & 0 & * \end{bmatrix}
	\end{align*}

-   A **lower triangular matrix** is defined as a matrix for which all
    entries **above** the main diagonal are equal to zero.
    
	\begin{align*}
    \begin{bmatrix}  * & 0 & \dots & 0 \\   * & 0 & \dots & \vdots \\   \vdots & \vdots & \ddots & 0 \\   * & \dots & * & * \end{bmatrix}
	\end{align*}

**Diagonal Matrices**: A **diagonal matrix** is defined as a matrix for which all entries
**above** and **below** the main diagonal are equal to zero.

\begin{align*}
\begin{bmatrix}  * & 0 & \dots & 0 \\   0 & * & \dots & \vdots \\   \vdots & \vdots & \ddots & 0 \\   0 & \dots & 0 & * \end{bmatrix}\end{align*}

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: Determinant of a Triangular Matrix
</b></font>
    
<p>If <span class="math inline">\(A\)</span> is a square triangular matrix, then <span class="math inline">\(\det(A)\)</span> is the product of the entries on the main diagonal.</p>


</div>

<font color='Blue'><b>Example</b></font>:
Let $A=\begin{bmatrix} 7 & 0 & 0 & 0 & 0 \\ 1 & \pi & 0 & 1 & 3 \\ 2 & 0 & 2 & -1 & 5 \\ 3 & 0 & 0 & 7 & 1 \\ 4 & 0 & 0 & 0 & 3\end{bmatrix}$. Find $\det(A)$

<font color='Green'><b>Solution</b></font>:
Expanding along row 1:
\begin{align*}
\det(A)=\left|\begin{array}{ccccc} 7 & 0 & 0 & 0 & 0\\ 1 & \pi  & 0 & 1 & 3\\ 2 & 0 & 2 & -1 & 5\\ 3 & 0 & 0 & 7 & 1\\ 4 & 0 & 0 & 0 & 3 \end{array}\right|
=7\left|\begin{array}{cccc} \pi  & 0 & 1 & 3\\ 0 & 2 & -1 & 5\\ 0 & 0 & 7 & 1\\ 0 & 0 & 0 & 3 \end{array}\right|
=(7)(\pi)( 2)(7)( 3)=294\pi.
\end{align*}
***

Properties of Determinants
-------------------------------

There are many important properties of determinants. Here, we discuss some important properties of determinants. We are familiar with the row operations:

<div class="alert alert-block alert-success">
<p>The row operations consist of the following</p>
<ol>
<li><p>Switching two rows.</p></li>
<li><p>Multiplying a row by a nonzero number.</p></li>
<li><p>Replacing a row by a multiple of another row added to itself.</p></li>
</ol>
</div>

We now consider the effect of row operations on the determinant of a matrix.

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem:
</b></font>
    
<p>Let <span class="math inline">\(B\)</span> be a matrix which results from …</p>
<ul>
<li><p>switching two rows of <span class="math inline">\(A\)</span>. Then <span class="math inline">\(det(B) = -det(A)\)</span>.</p></li>
<li><p>multiplying some row of <span class="math inline">\(A\)</span> by a scalar <span class="math inline">\(k\)</span>. Then <span class="math inline">\(\det(B) = k\det(A)\)</span>.</p></li>
<li><p>adding a multiple of a row to another row. Then <span class="math inline">\(det(B) = det(A)\)</span>.</p></li>
</ul>

</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark
</b></font>
    
Note that this theorem is true when we multiply one row of the matrix by $k$. If we were to multiply two rows of $A$ by $k$ to obtain $B$, we would have $\det(B) = k ^2 \det(A)$. Suppose we were to multiply all rows of $A$, where $A$ is a $n\times n$ matrix,  by $k$ to obtain the matrix $B$, so that $B = kA$. Then, $\det(B) = k^n \det(A)$.

</div>

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: Scalar Multiplication
</b></font>
    
<p>Let <span class="math inline">\(A\)</span> and <span class="math inline">\(B\)</span> be <span class="math inline">\(n\times n\)</span> matrices and <span class="math inline">\(k\)</span> a scalar, such that <span class="math inline">\(B = kA\)</span>. Then <span class="math inline">\(\det(B) = k^n \det(A)\)</span>.</p>

</div>

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem:
</b></font>
    
<ul>
<li><p><strong>Determinant of a Product:</strong> Let <span class="math inline">\(A\)</span> and <span class="math inline">\(B\)</span> be two <span class="math inline">\(n\times n\)</span> matrices. Then <span class="math display">\[\det(AB) = \det(A)\det(B).\]</span></p></li>
<li><p><strong>Determinant of the Transpose</strong>: Let <span class="math inline">\(A\)</span> be a matrix where <span class="math inline">\(A^T\)</span> is the transpose of <span class="math inline">\(A\)</span>. Then, <span class="math display">\[\det\left(A^T\right)= \det(A).\]</span></p></li>
<li><p><strong>Determinant of the Inverse:</strong> Let <span class="math inline">\(A\)</span> be an <span class="math inline">\(n\times n\)</span> matrix. Then <span class="math inline">\(A\)</span> is invertible if and only if <span class="math inline">\(\det(A) \neq 0\)</span>. If this is true, it follows that <span class="math display">\[\det(A^{-1}) =\det(A)^{-1}=\frac{1}{\det(A)}.\]</span></p></li>
</ul>

</div>

<font color='Blue'><b>Example</b></font>:
Suppose $A$, $B$ and $C$ are $4\times 4$ matrices and $\det(A)=-1$, $\det(B)>0$ and $\det(C)=\frac{1}{2}$. Find $\det(2\,A^2B^{-1}(C^T)^3BA^{-1})$.

***
Since $A$, $B$ and $C$ are $4\times 4$ matrices, $A^2B^{-1}(C^T)^3BA^{-1}$ is also a $4\times 4$ matrix.
\begin{align*}
\det(\underbrace{2}_{\text{\text{scalar}}}\,\underbrace{A^2B^{-1}(C^T)^3BA^{-1}}_{4\times 4\text{ matrix}})&=
2^4\,\det(A^2B^{-1}(C^T)^3BA^{-1})\\
&=16\,\det(A^2)\,\det(B^{-1})\,\det((C^T)^3)\,\det(B)\,\det(A^{-1})\\
&=16\,(\det(A))^2\,\frac{1}{\det(B)}\,(\det(C^T))^3\,\det(B)\,\frac{1}{\det(A)}\\
&=16\,(\det(A))^2\,(\det(C))^3\,\frac{1}{\det(A)}\\
&=16\,\det(A)\,(\det(C))^3\\
&=16\,(-1)\,(\frac{1}{2})^3\\
&=16\,(-1)\,\frac{1}{8}=-2
\end{align*}
***

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem:
</b></font>
    
<ul>
<li><p>If <span class="math inline">\(A\)</span> is an <span class="math inline">\(n\times n\)</span> matrix such that one of its rows consists of zeros, then <span class="math inline">\(\det(A) = 0\)</span>.</p></li>
<li><p>If two rows/columns of <span class="math inline">\(A\)</span> are identical then <span class="math inline">\(\det(A) = 0\)</span>.</p></li>
</ul>

</div>

## Finding Determinants using Row Operations

By using row operations, we can simplify a matrix to the point where we can find the determinant easily. We usually continue using row operations until the matrix is in a triangular form, and taken the product of the entries on the main diagonal.

<font color='Blue'><b>Example</b></font>:
Find $\det(A)$ if $A=\begin{bmatrix}3 & 1 & 2 & 7\\ 3 & 2 & 4 & 8\\ 3 & 1 & 7 & 9\\ 3 & 1 & 2 & 6\end{bmatrix}$.

<font color='Green'><b>Solution</b></font>:
Using row operations:
\begin{align*}
A=\left[\begin{array}{cccc} 3 & 1 & 2 & 7\\ 3 & 2 & 4 & 8\\ 3 & 1 & 7 & 9\\ 3 & 1 & 2 & 6 \end{array}\right]
&\Rightarrow[\text{No effect on det.}]{-R_{1}+R_{2}\rightarrow R_{2}} \Rightarrow \quad
\left[\begin{array}{cccc} 3 & 1 & 2 & 7\\ 0 & 1 & 2 & 1\\ 3 & 1 & 7 & 9\\ 3 & 1 & 2 & 6 \end{array}\right]
\\ &
\Rightarrow[\text{No effect on det.}]{-R_{1}+R_{3}\rightarrow R_{3}} \Rightarrow \quad
\left[\begin{array}{cccc} 3 & 1 & 2 & 7\\ 0 & 1 & 2 & 1\\ 0 & 0 & 5 & 2\\ 3 & 1 & 2 & 6 \end{array}\right]
\\ &
\Rightarrow[\text{No effect on det.}]{-R_{1}+R_{4}\rightarrow R_{4}} \Rightarrow \quad
\left[\begin{array}{cccc} 3 & 1 & 2 & 7\\ 0 & 1 & 2 & 1\\ 0 & 0 & 5 & 2\\ 0 & 0 & 0 & -1\end{array}\right]=R.
\end{align*}
Matrix $R$, the reduced matrix, is an upper triangular matrix. Therefore,
\begin{align*}
\det(A)=\det(R)
=(3)(1)(5)(-1)=-15.
\end{align*}

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
