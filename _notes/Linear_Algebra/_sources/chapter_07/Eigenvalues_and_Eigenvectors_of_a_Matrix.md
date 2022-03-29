# 7.1 Eigenvalues and Eigenvectors of a Matrix

## 7.1.1 Definition of Eigenvectors and Eigenvalues

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Eigenvalues and Eigenvectors of a Matrix
</b></font>
    
Let $A$ be an $n\times n$ matrix and let $X \in \mathbb{C}^n$  be a **nonzero vector** for which
\begin{align*}
AX = \lambda X
\end{align*}
for some scalar $\lambda$ . Then $\lambda$ is called an **eigenvalue** of the matrix $A$ and $X$ is called an **eigenvector** of
$A$ associated with $\lambda$, or a $\lambda$-eigenvector of $A$.
</div>

<font color='Blue'><b>Example</b></font>:
Let $A=\left[\begin{array}{cc} 2 & -2\\ -1 & 3 \end{array}\right]$ and $X=\left[\begin{array}{c} 2\\ 1 \end{array}\right]$.
Then
\begin{align*}
AX=\left[\begin{array}{cc} 2 & -2\\ -1 & 3 \end{array}\right]\left[\begin{array}{c} 2\\ 1 \end{array}\right]
=\left[\begin{array}{c} 2\\ 1 \end{array}\right]
\end{align*}
and
\begin{align*}
1 X=1 \left[\begin{array}{c} 2\\ 1 \end{array}\right]=\left[\begin{array}{c} 2\\ 1 \end{array}\right].
\end{align*}
Hence, $AX=1 X$. This means that $1$ is an {eigenvalue} of $A$, and
$\left[\begin{array}{c} 2\\ 1 \end{array}\right]$ is an **eigenvector of $A$ corresponding to $1$** (or a $1$-eigenvector of $A$).

<div class="alert alert-info" role="alert">
<font size="+1"><b>
The Spectrum of a Matrix
</b></font>
    
The set of all eigenvalues of an $n\times n$ matrix $A$ is denoted by
$\sigma(A)$ and is referred to as the **spectrum** of $A$.
</div>

Suppose that $A$ is an $n\times n$ matrix, with eigenvalue
$\lambda$ and corresponding eigenvector $X$.

Then, $X\neq 0$ is an $n$-vector, $\lambda\in \mathbb{R}$, and $AX=\lambda X$. It follows that
\begin{eqnarray*}
\lambda X - AX & = & 0 \\
\lambda I X - AX & = & 0 \\
(\lambda I - A)X & = & 0
\end{eqnarray*}


Since $X\neq 0$, $X$ is a \textbf{nontrivial} solution to the linear system with coefficient matrix $\lambda I-A$, and therefore the matrix **$\lambda I-A$ is not invertible**. Since a matrix is invertible if and only if its determinant is not equal to zero, it follows that
\begin{align*}
\det(\lambda I - A)=0.
\end{align*}

<div class="alert alert-info" role="alert">
<font size="+1"><b>
The Characteristic Polynomial and the Characteristic Equation
</b></font>
    
If $A$ is an $n\times n$  matrix, the characteristic polynomial $c_A (\lambda)$ of $A$ is defined by
\begin{align*}
c_A (\lambda) = \det(\lambda I-A).
\end{align*}
Moreover, $\det(\lambda I-A)=0$ is usually referred as the \textbf{characteristic equation}.
</div>


<font color='Blue'><b>Example</b></font>:
Find the characteristic polynomial of $A=\left[\begin{array}{cc} 2 & -2\\ -1 & 3 \end{array}\right]$.

<font color='Green'><b>Solution</b></font>:
\begin{align*}
c_A(\lambda) & = \det(\lambda I-A)
\\&
=\det\left(\left[\begin{array}{cc}\lambda & 0 \\ 0 & \lambda \end{array}\right] -\left[\begin{array}{cc} 2 & -2\\ -1 & 3 \end{array}\right]\right)
\\&
=\left|\begin{array}{cc} \lambda -2 & 2\\ 1 & \lambda -3 \end{array}\right|
\\&
=(\lambda -2)(\lambda -3)-(2)(1)=\lambda ^2-5\,\lambda +4
\end{align*}

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: The Existence of an Eigenvector
</b></font>
    
<p>Let <span class="math inline">\(A\)</span> be an <span class="math inline">\(n\times n\)</span> matrix and suppose<span class="math inline">\(c_A (\lambda)\)</span> = 0 for some <span class="math inline">\(\lambda \in \mathbb{C}\)</span>. Then <span class="math inline">\(\lambda\)</span> is an eigenvalue of <span class="math inline">\(A\)</span> and thus there exists a nonzero vector <span class="math inline">\(X \in C^n\)</span> such that <span class="math inline">\(AX = \lambda X\)</span>.</p>

</div>

## 7.1.2 Finding Eigenvectors and Eigenvalues

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: The Existence of an Eigenvector
</b></font>
    
<p>Let <span class="math inline">\(A\)</span> be an <span class="math inline">\(n\times n\)</span> matrix.</p>
<ol>
<li><p>The eigenvalues of <span class="math inline">\(A\)</span> are the roots of <span class="math inline">\(c_A(x)\)</span>.</p></li>
<li><p>The <span class="math inline">\(\lambda\)</span>-eigenvectors <span class="math inline">\(X\)</span> are the nontrivial solutions to <span class="math inline">\((\lambda I-A)X=0\)</span>.</p></li>
</ol>

</div>

<font color='Blue'><b>Example</b></font>:
Find the eigenvalues and eigenvectors of $A=\left[\begin{array}{cc} 2 & -2\\ -1 & 3 \end{array}\right]$.

<font color='Green'><b>Solution</b></font>:
In the last Example, for $A=\left[\begin{array}{cc} 2 & -2\\ -1 & 3 \end{array}\right]$, we found
\begin{align*}
\lambda ^2-5\,\lambda +4=(\lambda -1) (\lambda -4)
\end{align*}
Hence, $A$ has eigenvalues $\lambda_1=1$ and $\lambda_2=4$.

The $1$-eigenvectors of $A$ (meaning the eigenvectors of $A$ corresponding to $\lambda_1=1$) are found by solving the homogeneous system $(1I-A)X=0$.

This is the homogeneous system with coefficient matrix:
\begin{align*}
1I-A
= 1\left[\begin{array}{rr} 1 & 0 \\ 0 & 1 \end{array}\right]-\left[\begin{array}{rr} 2 & -2\\ -1 & 3 \end{array}\right]
=\left[\begin{array}{cc} -1 & 2 \\ 1 & -2 \end{array}\right].
\end{align*}
Solve the system in the standard way, by putting the augmented matrix of the system in reduced row-echelon form (RREF).
\begin{align*}
\left[\begin{array}{cc|c} -1 & 2 & 0\\ 1 & -2 & 0 \end{array}\right]
\Rightarrow\text{RREF} \Rightarrow
\left[\begin{array}{cc|c} 1 & -2 & 0\\ 0 & 0 & 0 \end{array}\right].
\end{align*}
The general solution is
\begin{align*}
X =\left[\begin{array}{c} 2t\\ t \end{array}\right]= t\left[\begin{array}{c} 2\\ 1 \end{array}\right]\mbox{ where } t\in\mathbb{R}.
\end{align*}
However, since eigenvectors are \textbf{nonzero}, the $1$-eigenvectors of $A$ are all vectors
\begin{align*}
X = t\left[\begin{array}{c} 2\\ 1 \end{array}\right] \mbox{ where } t\in\mathbb{R}\mbox{ and } t\neq 0.
\end{align*}

To find the $4$-eigenvectors of $A=\left[\begin{array}{rr} 2 & -2\\ -1 & 3 \end{array}\right]$, we solve the homogeneous system \linebreak $(4I-A)X=0$, with coefficient matrix
\begin{align*}
4I-A = 4\left[\begin{array}{cc} 1 & 0 \\ 0 & 1 \end{array}\right]-\left[\begin{array}{rr} 2 & -2\\ -1 & 3 \end{array}\right]
=\left[\begin{array}{rr} 2 & 2\\ 1 & 1 \end{array}\right].\end{align*}
and
\begin{align*}
\left[\begin{array}{cc|c} 2 & 2 & 0\\ 1 & 1 & 0 \end{array}\right]
\Rightarrow\text{RREF} \Rightarrow
\left[\begin{array}{cc|c} 1 & 1 & 0\\ 0 & 0 & 0 \end{array}\right].
\end{align*}
Therefore the $4$-eigenvectors of $A$ are the vectors
\begin{align*}
X = \left[\begin{array}{c} -s\\ s \end{array}\right]=s\left[\begin{array}{c} -1\\ 1 \end{array}\right]\mbox{ where } s\in\mathbb{R}\mbox{ and } s\neq 0.
\end{align*}

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Basic Eigenvector
</b></font>
    
A **basic eigenvector** of an $n\times n$ matrix $A$ is any nonzero multiple of a basic solution to $(\lambda I-A)X=0$, where $\lambda$ is
an eigenvalue of $A$.
</div>

<font color='Blue'><b>Example</b></font>:
Basic eigenvectors of
$A=\left[\begin{array}{rr} 2 & -2\\ -1 & 3 \end{array}\right]$:

-   $X = \left[\begin{array}{r} 2\\ 1 \end{array}\right]$ is is a basic
    eigenvector of $A$ corresponding to the eigenvalue $1$.

-   $X=\left[\begin{array}{r} -1 \\ 1 \end{array}\right]$ is a basic
    eigenvector of $A$ corresponding to the eigenvalue $4$.

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Multiplicity of an Eigenvalue
</b></font>
    
The multiplicity of an eigenvalue $\lambda$ of $A$ is the number of times $\lambda$ occurs as a root of $c_A(x)$.
</div>

<font color='Blue'><b>Example</b></font>:
Find the characteristic polynomial and eigenvalues of the matrix
\begin{align*}
A=\left[\begin{array}{rrr}
4 & 1 & 2 \\ 0 & 3 & -2 \\ 0 & -1 & 2
\end{array}\right].
\end{align*}

<font color='Green'><b>Solution</b></font>:

\begin{align*}
c_A(\lambda)=\det(\lambda I-A)
& = \det \left[\begin{array}{ccc}\lambda-4 & -1 & -2 \\ 0 & \lambda-3 & 2 \\ 0 & 1 & \lambda-2\end{array}\right]= (\lambda-4)[(\lambda-3)(\lambda-2)-2] \\
& =  (\lambda-4)(\lambda^2-5\lambda+4)=  (\lambda-4)(\lambda-4)(\lambda-1)\\
& =  (\lambda-4)^2(\lambda-1).
\end{align*}

Therefore, $A$ has eigenvalues $1$ and $4$, with $4$ being
an eigenvalue of **multiplicity two**.

<div class="alert alert-block alert-success">
<font size="+1"><b>
Finding Eigenvectors and Eigenvalues
</b></font>

Let $A$ be an $n\times n$ matrix.
* Find the eigenvalues $\lambda$ of $A$ by solving the characteristic equation, $\det(\lambda I-A)=0$.
* For each $\lambda$, find the basic eigenvectors $X\neq 0$ by finding the basic solutions to $(\lambda I-A)X =0$.
* To verify your work, make sure that $AX = \lambda X$ for each $\lambda$ and associated eigenvector $X$ .
</div>

<font color='Blue'><b>Example</b></font>:
Find the characteristic polynomial of the matrix $A =\begin{bmatrix} 2 & 2 & -2\\ 1 & 3 & -1\\ -1 & 1 & 1 \end{bmatrix}$, and then find all the eigenvalues and their eigenvectors.

<font color='Green'><b>Solution</b></font>:
The characteristic polynomial:
\begin{align*}
c_A (\lambda) &= \det(\lambda I-A)
= \left|\begin{array}{ccc} \lambda -2 & -2 & 2\\ -1 & \lambda -3 & 1\\ 1 & -1 & \lambda -1 \end{array}\right|
= \left|\begin{array}{ccc} \lambda -2 & -2 & 2\\ -1 & \lambda -3 & 1\\ 0 & \lambda -4 & \lambda  \end{array}\right|
\\ &
=(\lambda -2)\left|\begin{array}{cc} \lambda -3 & 1\\ \lambda -4 & \lambda  \end{array}\right|
-(-1)\left|\begin{array}{cc} -2 & 2\\ \lambda -4 & \lambda  \end{array}\right|
\\ &
=(\lambda -2)\left( \lambda(\lambda -3)- (\lambda -4)\right)+\left( -2\lambda - 2(\lambda -4)\right)
\\ &
=(\lambda -2)\left(\lambda^2 - 4\lambda + 4\right)+\left(8-4\,\lambda\right)
%\\ &
=(\lambda -2)\left(\lambda^2 - 4\lambda + 4\right)-4\left(\lambda-2\right)
\\ &
=(\lambda -2)\left(\lambda^2 - 4\lambda + 4-4\right)
%\\ &
=(\lambda -2)\left(\lambda^2 - 4\lambda\right)
=\lambda(\lambda - 2)(\lambda - 4).
\end{align*}
The eigenvalues of $A$ are the the roots of $c_A(\lambda)$:
\begin{align*}
&\lambda_1 = 0,~\lambda_2 = 4~\text{and}~\lambda_3 = 2.
\\ &
\sigma(A)=\{0,2,4\}.
\end{align*}

<div class="alert alert-danger" role="alert">
<p><span class="math inline">\(\lambda_1 = 0\)</span></p>
</div>

Finding the eigenvectors corresponding to $\lambda_1 = 0$:
\begin{align*}
&(\lambda_1 I-A)X =0,
\quad \Rightarrow   \quad
\left(0I-\begin{bmatrix} 2 & 2 & -2\\ 1 & 3 & -1\\ -1 & 1 & 1  \end{bmatrix} \right)X =\begin{bmatrix}0\\ 0\\0\end{bmatrix},
\quad \Rightarrow   \quad
\begin{bmatrix}-2 & -2 & 2\\ -1 & -3 & 1\\ 1 & -1 & -1\end{bmatrix}X =\begin{bmatrix}0\\ 0\\0\end{bmatrix}.
\end{align*}
The augmented matrix for finding the solutions is given by
\begin{align*}
\left[\begin{array}{ccc|c} -2 & -2 & 2 & 0\\ -1 & -3 & 1 & 0\\ 1 & -1 & -1 & 0 \end{array}\right]
\end{align*}
and the reduced row-echelon form of this matrix is
\begin{align*}
\left[\begin{array}{ccc|c} {1} & 0 & -1 & 0\\ 0 & {1} & 0 & 0\\ 0 & 0 & 0 & 0 \end{array}\right]
\end{align*}
Let $X=\begin{bmatrix}x & y & z\end{bmatrix}^T$. We can see that columns 1 and 2 are pivot columns. These columns correspond to variables $x$ and $y$,
making these the basic variables. Column 3 is not a pivot column, which means that $z$ is a free variable. We can write the solution to this system as
\begin{align*}
\begin{cases}z = t,\\x -t=0, \\y = 0.  \end{cases}
\end{align*}
Hence, the general solution $X$ to $(0 I-A)X =0$ is
\begin{align*}
t \begin{bmatrix} 1\\0\\1 \end{bmatrix},\quad t\neq0.
\end{align*}
Therefore, we can use
$X_1 = \begin{bmatrix} 1\\0\\1\end{bmatrix}$
as the basic eigenvector corresponding to
$\lambda_1 = 0$.

<div class="alert alert-danger" role="alert">
<p><span class="math inline">\(\lambda_2 = 4\)</span></p>
</div>

We have,
\begin{align*}
&(\lambda_2 I-A)X =0,
\quad \Rightarrow   \quad
\left(4I-\begin{bmatrix} 2 & 2 & -2\\ 1 & 3 & -1\\ -1 & 1 & 1  \end{bmatrix} \right)X =\begin{bmatrix}0\\ 0\\0\end{bmatrix},
\quad \Rightarrow   \quad
\begin{bmatrix}2 & -2 & 2\\ -1 & 1 & 1\\ 1 & -1 & 3\end{bmatrix}X =\begin{bmatrix}0\\ 0\\0\end{bmatrix}.
\end{align*}
The augmented matrix:
\begin{align*}
\left[\begin{array}{ccc|c} 2 & -2 & 2 & 0\\ -1 & 1 & 1 & 0\\ 1 & -1 & 3 & 0 \end{array}\right]
\end{align*}
and the reduced row-echelon form:
\begin{align*}
\left[\begin{array}{ccc|c} {1} & -1 & 0 & 0\\ 0 & 0 & {1} & 0\\ 0 & 0 & 0 & 0 \end{array}\right]
\end{align*}
Let $X=\begin{bmatrix}x & y & z\end{bmatrix}^T$. We can see that columns 1 and 3 are pivot column. These columns correspond to variables $x$ and $z$,
making these the basic variables. Column 2 is not a pivot column, which means that $y$ is a free variable. We can write the solution to this system as

\begin{align*}
\begin{cases}y = t,\\x -t=0, \\z = 0.  \end{cases}
\end{align*}
Hence, the general solution $X$ to $(4 I-A)X =0$ is
\begin{align*}
t \begin{bmatrix} 1\\1\\0 \end{bmatrix},\quad t\neq0.
\end{align*}
Therefore, we can use
$X_2 = \begin{bmatrix} 1\\1\\0\end{bmatrix}$ as the basic eigenvector corresponding to $\lambda_2 = 4$.

<div class="alert alert-danger" role="alert">
<p><span class="math inline">\(\lambda_3 = 2\)</span></p>
</div>

Finally,
\begin{align*}
&(\lambda_3 I-A)X =0,
\quad \Rightarrow   \quad
\left(2I-\begin{bmatrix} 2 & 2 & -2\\ 1 & 3 & -1\\ -1 & 1 & 1  \end{bmatrix} \right)X =\begin{bmatrix}0\\ 0\\0\end{bmatrix},
\quad \Rightarrow   \quad
\begin{bmatrix} 0 & -2 & 2\\ -1 & -1 & 1\\ 1 & -1 & 1\end{bmatrix}X =\begin{bmatrix}0\\ 0\\0\end{bmatrix}.
\end{align*}
The augmented matrix:
\begin{align*}
\left[\begin{array}{ccc|c} 0 & -2 & 2 & 0\\ -1 & -1 & 1 & 0\\ 1 & -1 & 1 & 0 \end{array}\right]
\end{align*}
and the reduced row-echelon form:
\begin{align*}
\left[\begin{array}{ccc|c} {1} & 0 & 0 & 0\\ 0 & {1} & -1 & 0\\ 0 & 0 & 0 & 0 \end{array}\right]
\end{align*}
Let $X=\begin{bmatrix}x & y & z\end{bmatrix}^T$. You can see that columns 1 and 2 are pivot columns. These columns correspond to variables $x$ and $y$,
making these the basic variables. Column 3 is not a pivot column, which means that $z$ is a free variable. We can write the solution to this system as
\begin{align*}
\begin{cases}z = t,\\y -t=0, \\x = 0.  \end{cases}
\end{align*}
Hence, the general solution $X$ to $(2 I-A)X =0$ is
\begin{align*}
t \begin{bmatrix} 0\\1\\1 \end{bmatrix},\quad t\neq0.
\end{align*}
Therefore, we can use
$X_3 = \begin{bmatrix} 0\\1\\1\end{bmatrix}$
as the basic eigenvector corresponding to
$\lambda_3 = 2$.

***

<font color='Blue'><b>Example</b></font>:
Let $A =\begin{bmatrix} 4 & 1 & 2\\ 0 & 3 & -2\\ 0 & -1 & 2 \end{bmatrix}$. Find the eigenvalues and eigenvectors of $A$.


<font color='Green'><b>Solution</b></font>:
The characteristic polynomial:
\begin{align*}
c_A (\lambda) &= \det(\lambda I-A)=\det\left(\begin{bmatrix}
\lambda -4 & -1 & -2\\ 0 & \lambda -3 & 2\\ 0 & 1 & \lambda -2
\end{bmatrix} \right)=(\lambda -4)
\left|\begin{array}{cc} \lambda -3 & 2\\ 1 & \lambda -2 \end{array}\right|
\\&=(\lambda -4)\left((\lambda -3)(\lambda -2)-2\right)
\\&=(\lambda -4)(\lambda ^2-5\,\lambda +4)=
(\lambda - 1)(\lambda - 4)^2.
\end{align*}
The eigenvalues of $A$ are the the roots of $c_A(\lambda)$:
\begin{align*}
&\lambda_1 = 1 \quad \text{and} \quad  \lambda_2=\lambda_3 = 4.
\\&
\sigma(A)=\{1,4\}.
\end{align*}

<div class="alert alert-danger" role="alert">
<p><span class="math inline">\(\lambda_1 = 1\)</span></p>
</div>

Finding the eigenvectors corresponding to $\lambda_1 = 1$:
\begin{align*}
&(\lambda_1 I-A)X =0,
\quad \Rightarrow   \quad
\left(I-\begin{bmatrix} 4 & 1 & 2\\ 0 & 3 & -2\\ 0 & -1 & 2   \end{bmatrix} \right)X =\begin{bmatrix}0\\ 0\\0\end{bmatrix},
\quad \Rightarrow   \quad
\begin{bmatrix}-3 & -1 & -2\\ 0 & -2 & 2\\ 0 & 1 & -1 \end{bmatrix}X =\begin{bmatrix}0\\ 0\\0\end{bmatrix}.
\end{align*}
The augmented matrix for finding the solutions is given by
\begin{align*}
\left[\begin{array}{ccc|c} -3 & -1 & -2 & 0\\ 0 & -2 & 2 & 0\\ 0 & 1 & -1 & 0 \end{array}\right]
\end{align*}
and the reduced row-echelon form of this matrix is
\begin{align*}
\left[\begin{array}{ccc|c} {1} & 0 & 1 & 0\\ 0 & {1} & -1 & 0\\ 0 & 0 & 0 & 0 \end{array}\right]
\end{align*}
Let $X=\begin{bmatrix}x & y & z\end{bmatrix}^T$. It can be seen that columns 1 and 2 are pivot columns. These columns correspond to variables $x$ and $y$,
making these the basic variables. Column 3 is not a pivot column, which means that $z$ is a free variable. We can write the solution to this system as
\begin{align*}
\begin{cases}z = t,\\x +t=0, \\y-t = 0.  \end{cases}
\end{align*}
Hence, the general solution $X$ to $(I-A)X =0$ is
\begin{align*}
t \begin{bmatrix} -1\\1\\1 \end{bmatrix},\quad t\neq0.
\end{align*}
Therefore, we can use
$X_1 = \begin{bmatrix} -1\\1\\1 \end{bmatrix}$
as the basic eigenvector corresponding to
$\lambda_1 = 1$.

<div class="alert alert-danger" role="alert">
<p><span class="math inline">\(\lambda_2 =\lambda_3= 4\)</span></p>
</div>

Similarly,
\begin{align*}
&(\lambda_2 I-A)X =0,
\quad \Rightarrow   \quad
\left(4I-\begin{bmatrix} 4 & 1 & 2\\ 0 & 3 & -2\\ 0 & -1 & 2  \end{bmatrix} \right)X =\begin{bmatrix}0\\ 0\\0\end{bmatrix},
\quad \Rightarrow   \quad
\begin{bmatrix}0 & -1 & -2\\ 0 & 1 & 2\\ 0 & 1 & 2 \end{bmatrix}X =\begin{bmatrix}0\\ 0\\0\end{bmatrix}.
\end{align*}
The augmented matrix:
\begin{align*}
\left[\begin{array}{ccc|c} 0 & -1 & -2 & 0\\ 0 & 1 & 2 & 0\\ 0 & 1 & 2 & 0 \end{array}\right]
\end{align*}
and the reduced row-echelon form:
\begin{align*}
\left[\begin{array}{ccc|c} 0 & {1} & 2 & 0\\ 0 & 0 & 0 & 0\\ 0 & 0 & 0 & 0 \end{array}\right]
\end{align*}
Let $X=\begin{bmatrix}x & y & z\end{bmatrix}^T$. Here, column 2 is the only pivot column. This column corresponds to variables $y$. Columns 1 and 3 are not pivot columns, which means that $x$ and $z$ are free variables. We can write the solution to this system as
\begin{align*}
\begin{cases}x=t,\\y +2s=0,\\z = s.  \end{cases}
\end{align*}
Hence, the general solution $X$ to $(4I-A)X =0$ is
\begin{align*}
\begin{bmatrix} t\\-2s\\s \end{bmatrix},\quad t,s\neq0
\quad \text{or} \quad
t \begin{bmatrix} 1\\0\\0 \end{bmatrix}+s \begin{bmatrix} 0\\-2\\1 \end{bmatrix},\quad t,s\neq0.
\end{align*}
Therefore, we can use $X_2 =\begin{bmatrix} 1\\0\\0\end{bmatrix}$ and $X_3 =\begin{bmatrix} 0\\-2\\1\end{bmatrix}$ as the basic eigenvectors corresponding to $\lambda_2 = \lambda_3=4$.
***

## 7.1.3 Eigenvalues and Eigenvectors for Special Types of Matrices


Let $A$, and $B$ be $n \times n$ matrices. Suppose there exists an invertible matrix $P$ such that
\begin{align*}
A = P^{-1} BP
\end{align*}
Then $A$ and $B$ are called \textbf{similar matrices}.

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem
</b></font>
    
Let $A$ and $B$ be similar matrices, so that $A = P^{-1}BP$ where $A$ and $B$ are $n\times n$ matrices, and $P$ is **invertible**. Then $A$ and $B$ have the **same eigenvalues**.
</div>

**Proof**: 
Assume $BX=\lambda X$. Let $Y=P^{-1}X$. Then
\begin{align*}
AY=(P^{-1}B P) P^{-1} X=P^{-1}B (P P^{-1}) X=P^{-1}BI X=P^{-1} BX=P^{-1} \lambda X=\lambda Y.
\end{align*}

It is possible to use elementary matrices to simplify a matrix before searching for its eigenvalues and
eigenvectors. This is illustrated in the following example.

<font color='Blue'><b>Example</b></font>:
Find the eigenvalues for the matrix
\begin{align*}
A =
\left[
\begin{array}{rrr}
33 & 105 & 105 \\
10 & 28 & 30 \\
-20 & -60 & -62
\end{array}
\right]
\end{align*}.


<font color='Green'><b>Solution</b></font>:
We will use elementary matrices to simplify $A$ before finding the eigenvalues. Right multiply $A$ by $E_{1}=E(-2\times 2+3)$, and left multiply $A$ by the inverse of $E_{1}$.
\begin{align*}
\underbrace{\left[\begin{array}{rrr}1 & 0 & 0 \\0 & 1 & 0 \\0 & 2 & 1\end{array}\right]}_{\color{red}{E_{1}^{-1}}}
\left[\begin{array}{rrr}33 & 105 & 105 \\10 & 28 & 30 \\-20 & -60 & -62\end{array}\right]
\underbrace{\left[\begin{array}{rrr}1 & 0 & 0 \\0 & 1 & 0 \\0 & -2 & 1\end{array}\right]}_{\color{red}{E_{1}}}
=\left[\begin{array}{rrr}33 & -105 & 105 \\10 & -32 & 30 \\0 & 0 & -2\end{array}\right].
\end{align*}
Note that the resulting matrix and $A$ are similar matrices (with $E_1$ playing the role of $P$) so they have the same eigenvalues.

We do this step again, on the resulting matrix above. This time, right multiply $A$ by\linebreak $E_{2}=E(3\times 2+1)$, and left multiply $A$ by the inverse of $E_{2}$.
\begin{align*}
\underbrace{\left[\begin{array}{rrr}1 & -3 & 0 \\0 &  1 & 0 \\0 &  0 & 1\end{array}\right]}_{\color{red}{E_{2}^{-1}}}
\left[\begin{array}{rrr}33 & -105 & 105 \\10 & -32  & 30 \\0  &   0  & -2\end{array}\right]
\underbrace{\left[\begin{array}{rrr}1 & 3 & 0 \\0 & 1 & 0 \\0 & 0 & 1\end{array}\right]}_{\color{red}{E_{2}}}
=\left[\begin{array}{rrr}3  & 0  & 15 \\10 & -2 & 30 \\0  & 0  & -2\end{array}\right] = B
\end{align*}
Again by properties of similar matrices, the resulting matrix here (labeled $B$) has the same eigenvalues as our original matrix $A$. The advantage is that it is much simpler to find the eigenvalues of $B$ than $A$.

Finding these eigenvalues follows the usual procedure and is left as an exercise.
***

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
The eigenvalues of a triangular matrix are the entries on the main diagonal.
</div>

<font color='Blue'><b>Example</b></font>:
Consider the matrix
\begin{align*}
A=\left[\begin{array}{cccc} 1 & -1 & 0 & 3\\ 0 & 2 & 1 & -2\\ 0 & 0 & 3 & 5\\ 0 & 0 & 0 & 4 \end{array}\right]
\end{align*}

The characteristic polynomial of $A$ is
\begin{align*} c_A(\lambda)=\det(\lambda I-A)=
\left|\begin{array}{cccc} \lambda -1 & 1 & 0 & -3\\ 0 & \lambda -2 & -1 & 2\\ 0 & 0 & \lambda -3 & -5\\ 0 & 0 & 0 & \lambda -4 \end{array}\right|=
(\lambda -1) ( \lambda -2 )( \lambda -3) ( \lambda -4)
\end{align*}
Therefore the eigenvalues of $A$ are $1, 2, 3$ and $4$, exactly the entries on the main diagonal of $A$.
***

<font color='Blue'><b>Example</b></font>:
Find the eigenvalues for the matrix
\begin{align*}
A =
\left[
\begin{array}{rrr}
33 & 105 & 105 \\
10 & 28 & 30 \\
-20 & -60 & -62
\end{array}
\right]
\end{align*}.


<font color='Green'><b>Solution</b></font>:
We will use elementary matrices to simplify $A$ before finding the eigenvalues. Right multiply $A$ by $E_{1}=E(-2\times 2+3)$, and left multiply $A$ by the inverse of $E_{1}$.
\begin{align*}
\underbrace{\left[\begin{array}{rrr}1 & 0 & 0 \\0 & 1 & 0 \\0 & 2 & 1\end{array}\right]}_{\color{red}{E_{1}^{-1}}}
\left[\begin{array}{rrr}33 & 105 & 105 \\10 & 28 & 30 \\-20 & -60 & -62\end{array}\right]
\underbrace{\left[\begin{array}{rrr}1 & 0 & 0 \\0 & 1 & 0 \\0 & -2 & 1\end{array}\right]}_{\color{red}{E_{1}}}
=\left[\begin{array}{rrr}33 & -105 & 105 \\10 & -32 & 30 \\0 & 0 & -2\end{array}\right].
\end{align*}
Note that the resulting matrix and $A$ are similar matrices (with $E_1$ playing the role of $P$) so they have the same eigenvalues.

We do this step again, on the resulting matrix above. This time, right multiply $A$ by\linebreak $E_{2}=E(3\times 2+1)$, and left multiply $A$ by the inverse of $E_{2}$.
\begin{align*}
\underbrace{\left[\begin{array}{rrr}1 & -3 & 0 \\0 &  1 & 0 \\0 &  0 & 1\end{array}\right]}_{\color{red}{E_{2}^{-1}}}
\left[\begin{array}{rrr}33 & -105 & 105 \\10 & -32  & 30 \\0  &   0  & -2\end{array}\right]
\underbrace{\left[\begin{array}{rrr}1 & 3 & 0 \\0 & 1 & 0 \\0 & 0 & 1\end{array}\right]}_{\color{red}{E_{2}}}
=\left[\begin{array}{rrr}3  & 0  & 15 \\10 & -2 & 30 \\0  & 0  & -2\end{array}\right] = B
\end{align*}
Again by properties of similar matrices, the resulting matrix here (labeled $B$) has the same eigenvalues as our original matrix $A$. The advantage is that it is much simpler to find the eigenvalues of $B$ than $A$.

Finding these eigenvalues follows the usual procedure and is left as an exercise.
***

<font color='Blue'><b>Example</b></font>:
For the matrix $A$ below, find a value of $k$ so that $A$ has two basic eigenvectors associated with the eigenvalue $\lambda = 2$.
\begin{align*}
A=\left[\begin{array}{cccc} 2 & 3 & -6 & k\\ 0 & -1 & 6 & 12\\ 0 & 0 & -3 & -15\\ 0 & 0 & 0 & 2 \end{array}\right]
\end{align*}


<font color='Green'><b>Solution</b></font>:
Since $\lambda$ is an eigenvalue of $A$, for a nonzero vector $X=\begin{bmatrix} x_1 & x_2 & x_3 & x_4 \end{bmatrix}^T$, we have
\begin{align*}
&(2I-A)X=0,
\\
&\left[\begin{array}{cccc} 0 & -3 & 6 & -k\\ 0 & 3 & -6 & -12\\ 0 & 0 & 5 & 15\\ 0 & 0 & 0 & 0 \end{array}\right]
\begin{bmatrix} x_1 \\ x_2 \\ x_3 \\ x_4 \end{bmatrix}
=\left[\begin{array}{c} 0\\ 0\\ 0\\ 0 \end{array}\right]
\end{align*}
The corresponding augmented matrix:
\begin{align*}
&\left[\begin{array}{cccc|c} 0 & -3 & 6 & -k & 0\\ 0 & 3 & -6 & -12 & 0\\ 0 & 0 & 5 & 15 & 0\\ 0 & 0 & 0 & 0 & 0 \end{array}\right]\\
\frac{1}{3}R_2\to R_2, \frac{1}{5}R_3\to R_3 \Rightarrow\quad &
\left[\begin{array}{cccc|c} 0 & -3 & 6 & -k & 0\\ 0 & 1 & -2 & -4 & 0\\ 0 & 0 & 1 & 3 & 0\\ 0 & 0 & 0 & 0 & 0 \end{array}\right]
\\ 
\Rightarrow\quad R_1+3R_2\to R_1 \Rightarrow\quad &
\left[\begin{array}{cccc|c} 0 & 0 & 0 & -k-12 & 0\\ 0 & 1 & -2 & -4 & 0\\ 0 & 0 & 1 & 3 & 0\\ 0 & 0 & 0 & 0 & 0 \end{array}\right]
\\ 
\Rightarrow\quad R_2+2R_3\to R_2 \Rightarrow\quad &
\left[\begin{array}{cccc|c} 0 & 0 & 0 & -k-12 & 0\\ 0 & {1} & 0 & 2 & 0\\ 0 & 0 & {1} & 3 & 0\\ 0 & 0 & 0 & 0 & 0 \end{array}\right]
\end{align*}
We can see that this system has two eigenvectors only if the RREF has two rows of zero. This means $-k-12=0$ and $k=-12$.

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***