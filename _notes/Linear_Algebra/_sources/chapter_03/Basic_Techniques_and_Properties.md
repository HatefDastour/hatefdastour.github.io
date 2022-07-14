# Basic Techniques and Properties

## Cofactors and Determinants


<div class="alert alert-info" role="alert">
<font size="+1"><b>
Determinant
</b></font>

The determinant of an $n\times n$ matrix $A$ is a number associated with $A$, and it is denoted by $\det(A)$ or $|A|$.
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Determinant of a Two By Two Matrix
</b></font>

If $A=\begin{bmatrix}a & b \\ c & d\end{bmatrix}$ (a $2\times 2$ matrix), the determinant is given by the following formula.
\begin{align*}
\det(A)=\left|\begin{array}{cc} a & b \\ c & d \end{array}\right|= ad-cb
\end{align*}
</div>



<font color='Blue'><b>Example</b></font>:
Find $det(A)$ for the matrix $A = \begin{bmatrix}1 & 2\\ 5 & 1\end{bmatrix}$.

<font color='Green'><b>Solution</b></font>: $\det(A)=(1)(1)-(2)(5)=1-10=-9.$


<div class="alert alert-info" role="alert">
<font size="+1"><b>
${ij}^{th}$ Minor of a Matrix
</b></font>

For a $3\times 3$ matrix $A$ , the $ij^{\text{th}}$ minor of $A$, indicated by $minor(A)_{ij}$, is the determinant of the $2\times 2$ matrix that is the result of deleting the $i^{\text{th}}$ row and the $j^{\text{th}}$ column of $A$.
</div>

In general, for an an $n\times n$ matrix $A$, the $ij^{\text{th}}$ minor of $A$ is the determinant of \linebreak the $(n-1)\times(n-1)$ matrix which results from deleting the $i^{\text{th}}$ row and the $j^{\text{th}}$ column of $A$.

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

<div class="alert alert-info" role="alert">
<font size="+1"><b>
${ij}^{th}$ Cofactor of a Matrix
</b></font>

For an an $n\times n$ matrix $A$, the $ij^{\text{th}}$ **cofactor**, denoted by $cof (A)_{ij}$, is defined by
\begin{align*}
cof (A) _{ij} = (-1)^{i+j} minor(A)_{ij}
\end{align*}
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark
</b></font>
    
* We use cofactors to compute the determinant of a matrix.
* $cof (A) _{ij}$ provides the sign of ($i$,$j$)-entry of $A$ multiplied by $minor(A)_{ij}$.
* Sign patterns:
\begin{align*}
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
\end{array}\right],\ldots
\end{align*}
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
The Determinant of a Three By Three Matrix
</b></font>

Let $a_{i1}$, $a_{i2}$, and $a_{i3}$ represent the entries on a row of $3\times 3$ matrix $A$, the determinant of $A$, $\det(A)$, can be calculated as follows,

\begin{align*}
det(A) = a_{i1}\, cof (A)_{i1} +a_{i2}\, cof (A)_{i2} +a_{i3}\, cof (A)_{i3}
\end{align*}

Note that the above determinant can also be calculated using a column of $3\times 3$ matrix $A$ similarly. 
</div>

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

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: The Determinant is Well Defined
</b></font>
    
In calculating the determinant of a $n\times n$ matrix, expanding the matrix along any row or column always gives the **same answer**.
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark
</b></font>

For convenience, we usually pick a row or column with **most zeros** for evaluating the determinant of a matrix.
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
\\ &
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

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Triangular Matrices
</b></font>

- An **upper triangular matrix** is defined as a matrix for which all entries **under** the main diagonal are equal to zero.
    
\begin{align*}
\begin{bmatrix}  * & * & \dots & * \\   0 & * & \dots & \vdots \\   \vdots & \vdots & \ddots & * \\   0 & \dots & 0 & * \end{bmatrix}
\end{align*}

- A **lower triangular matrix** is defined as a matrix for which all entries **above** the main diagonal are equal to zero.
    
\begin{align*}
\begin{bmatrix}  * & 0 & \dots & 0 \\   * & 0 & \dots & \vdots \\   \vdots & \vdots & \ddots & 0 \\   * & \dots & * & * \end{bmatrix}
\end{align*}

A **triangular matrix** is a matrix that is either an upper triangular matrix or a lower triangular matrix.
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Diagonal Matrices
</b></font>

A **diagonal matrix** has zero entries everywhere except its main diagonal.

\begin{align*}
\begin{bmatrix}  * & 0 & \dots & 0 \\   0 & * & \dots & \vdots \\   \vdots & \vdots & \ddots & 0 \\   0 & \dots & 0 & * \end{bmatrix}
\end{align*}
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Determinant of a Triangular Matrix
</b></font>
    
For a square triangular matrix $A$, the determinant of $A$ is the product of the entries on the main diagonal. That is
\begin{align*}
\left|\begin{array}{cccc}  a_{11} & 0 & \dots & 0 \\   0 & a_{22} & \dots & \vdots \\   \vdots & \vdots & \ddots & 0 \\   0 & \dots & 0 & a_{nn} \end{array}\right| = a_{11}\,a_{22}\,\dots\,a_{nn}
\end{align*}

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

## Properties of Determinants
Here, we discuss some important properties of determinants. We are familiar with the row operations including


* Swapping two rows.
* Multiplying a row by a nonzero number.
* Substituting a row by adding another row multiplied by a number to it.

What would be the potential effect of row operations on the determinant of a matrix?

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem:
</b></font>
    
Let $B$ be a matrix which results from $\ldots$
* switching two rows of $A$. Then, $det(B) = -det(A)$.
* multiplying a row of $A$ by a scalar $k$. Then, $\det(B) = k\det(A)$.
* adding a multiple of a row to another row. Then, $det(B) = det(A)$.
</ul>

</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark
</b></font>
    
In case matrix $B$ is obtained by multiplying two rows of $A$ by $k$, then $\det(B) = k ^2 \det(A)$. Similarly, if $B$ is obtained by multiplying $n$ rows of $A$ by $k$, then $\det(B) = k ^n \det(A)$.
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Scalar Multiplication
</b></font>
    
If $B$ (a $n\times n$ matrix) is obtained through multiplying a $n\times n$ matrix $A$ by $k$, then $\det(B) = k^n \det(A)$.
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem:
</b></font>
    
* \textbf{Determinant of a Product:} the determinant of the product of matrix $A$ and matrix $B$ is the product of determinant of $A$ and determinant of $B$:
\begin{align*}
\det(AB) = \det(A)\det(B).
\end{align*}
* \textbf{Determinant of the Transpose}:the determinant of $A^T$ is the same as the determinant of matrix $A$.
\begin{align*}\det\left(A^T\right)= \det(A).\end{align*}
* \textbf{Determinant of the Inverse:} A $n\times n$ matrix $A$ is invertible if and only if $\det(A) \neq 0$, and
\begin{align*}\det(A^{-1}) =\det(A)^{-1}=\frac{1}{\det(A)}.\end{align*}
</div>

<font color='Blue'><b>Example</b></font>:
Suppose $A$, $B$ and $C$ are $4\times 4$ matrices and $\det(A)=-1$, $\det(B)>0$ and $\det(C)=\frac{1}{2}$. Find $\det(2\,A^2B^{-1}(C^T)^3BA^{-1})$.

<font color='Green'><b>Solution</b></font>:
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

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem:
</b></font>
    
* If an entire row of matrix $A$ is zero, then$\det(A) = 0$.
* If a rows or columns of matrix $A$ is repeated more than once, then  $\det(A) = 0$.

</div>

## 3.1.4 Finding Determinants using Row Operations

Using row operations can make calculating determinants a bit more convenient. The ideal scenario would be turning a matrix into a triangular matrix and calculating its determinant by multiplying entries on its main diagonal.

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
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***