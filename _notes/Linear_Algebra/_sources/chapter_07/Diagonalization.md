# 7.2 Diagonalization

## 7.2.1 Similarity and Diagonalization

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Trace of a Matrix
</b></font>
    
The trace of an $n\times n$ matrix $A$ is defined to be the sum of the
main diagonal elements of $A$
\begin{align*}
tr(A) = \sum_{i=1}^{n}a_{ii}.
\end{align*}
</div>

<font color='Blue'><b>Example</b></font>:
Find the trace of a matrix of $A=\left[\begin{array}{ccc} 1 & 1 & 2\\ 3 & 4 & 5\\ 1 & 2 & 3 \end{array}\right]$.

<font color='Green'><b>Solution</b></font>:
The trace of $A$:
\begin{align*}
tr(A)=1+4+3=8.
\end{align*}

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Properties of Trace
</b></font>
    
For $n\times n$ matrices $A$ and $B$, and any $k \in \mathbb{R}$,
* $tr (A+B) = tr (A)+ tr (B)$,
* $tr (kA) = k\, tr (A)$
* $tr (AB) = tr (BA)$
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Similar Matrices
</b></font>
    
If $A$ and $B$ be $n\times n$, we say that $A$ and $B$ are similar, and write $A \sim B$, if $B = P^{-1} AP$ for some invertible matrix $P$.
</div>


<div class="alert alert-block alert-success">
<font size="+1"><b>
Lemma: Similarity is an Equivalence Relation
</b></font>
    
Similarity is an equivalence relation, i.e. for $n\times n$ matrices $A$, $B$, and $C$,
* $A \sim A$, \hfill(reflexive)
* If $A \sim B$, then $B \sim A$,\hfill(symmetric)
* If $A \sim B$ and $B \sim C$ , then $A \sim C$,\hfill(transitive)
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Properties of Similar Matrices
</b></font>
    
If $A$ and $B$ are $n\times n$ matrices and $A \sim B$, then
* $\det(A)=\det(B)$,
* $rank(A)=rank(B)$,
* $tr (A) = tr (B)$,
* $c_A (\lambda) = c_B (\lambda)$,\hfill ($A$ and $B$ have the same characteristic polynomial).
* $\sigma(A)=\sigma(B)$,\hfill($A$ and $B$ have the same eigenvalues).
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Diagonal Matrix
</b></font>
    
An $n\times n$ matrix $A$ is diagonal if it is both upper triangular and lower triangular.

Equivalently, all entries except those on the main diagonal are zeros.

An $n\times n$ diagonal matrix:
\begin{align*}
D=
\left[\begin{array}{cccccc}
{\color{red} a_{1}} & 0 & 0 & \cdots & 0 & 0 \\
0 & {\color{red}a_{2}}  & 0 & \cdots & 0 & 0 \\
0 & 0 & {\color{red} a_{2}}  & \cdots & 0 & 0 \\
\vdots & \vdots & \vdots & \vdots & \vdots & \vdots \\
0 & 0 & 0 & \cdots & {\color{red} a_{n-1}} & 0\\
0 & 0 & 0 & \cdots & 0 & {\color{red}a_{n}}
\end{array}\right]
\end{align*}
is written $D=\mathrm{Diag}(a_1, a_2, a_3, \ldots, a_{n-1}, a_n)$.
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Diagonalizable
</b></font>
    
Let $A$ be an $n\times n$ matrix. Then $A$ is said to be \textbf{diagonalizable} if there exists an invertible matrix $P$
such that $P^{-1} AP = D$ where $D$ is a diagonal matrix.
\\~\\
Here the invertible matrix $P$ is called a \textbf{diagonalizing matrix} for $A$.
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Proposition:
</b></font>
    
An $n\times n$ matrix $A$ is \textbf{diagonalizable} if $A\sim D$ for some \textbf{diagonal matrix} $D$.
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Dominant Eigenvalue
</b></font>
    
If $\lambda$ is an eigenvalue of $A$ that is larger in absolute value
than any other eigenvalue, it is called the **dominant eigenvalue** of
$A$.
</div>

Note that the above equation can be rearranged as $A = PDP^{-1}$ . Suppose we wanted to compute $A^{100}$. By diagonalizing A first it suffices to then compute $\left(PDP^{-1}\right)^{100}$, which reduces to $PD^{100} P^{-1}$. This last computation is much simpler than $A^{100}$.

## 7.2.2 Diagonalizing a Matrix

Let $A$ be an $n\times n$ matrix. The process of finding an
**invertible** matrix $P$ and a **diagonal** matrix $D$ so that
$A=PDP^{-1}$ is referred to as **diagonalizing** the matrix $A$, and $P$
is called the **diagonalizing** matrix for $A$.

The key to diagonalizing a matrix (finding the matrices $P$ and $D$)
lies in the eigenvectors and eigenvalues of the matrix $A$.

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Eigenvectors and Diagonalizable Matrices
</b></font>
    
Let $A$ be an $n\times n$ matrix.
1. $A$ is diagonalizable if and only if it has eigenvectors $X_1, X_2, \ldots, X_n$ so that \linebreak
$P = \left[\begin{array}{cccc} X_1 & X_2 & \cdots & X_n \end{array}\right]$ is invertible.

2. If $P$ is invertible, then
\begin{align*}P^{-1}AP=\mathrm{Diag}(\lambda_1, \lambda_2, \ldots, \lambda_n )\end{align*}
where $\lambda_i$ is the eigenvalue of $A$ corresponding to
the eigenvector $X_i$, i.e., $AX_i=\lambda_i X_i$.
</div>

<font color='Blue'><b>Example</b></font>:
Let
$A =\left[\begin{array}{ccc} 1 & 1 & 0\\ 0 & 2 & 0\\ 0 & 2 & 1 \end{array}\right]$.
Find an invertible matrix $P$ and a diagonal matrix $D$ such that
$P^{-1}AP = D$.

<font color='Green'><b>Solution</b></font>:
The characteristic polynomial:
\begin{align*}
c_A (\lambda) &= \det(\lambda I-A)=
\left|\begin{array}{ccc} \lambda -1 & -1 & 0\\ 0 & \lambda -2 & 0\\ 0 & -2 & \lambda -1 \end{array}\right|
\\&=
(\lambda -1)\left|\begin{array}{cc} \lambda -2 & 0\\ -2 & \lambda -1 \end{array}\right| \\&=
(\lambda - 2)(\lambda - 1)^2
\end{align*}
The eigenvalues of $A$ are the the roots of $c_A(\lambda)$:
\begin{align*}
\lambda_1 =\lambda_2= 1 \quad \text{and} \quad  \lambda_3 = 2.
\end{align*}
Note that here $2$ is the dominant eigenvalue of $A$ since $|\lambda_3|=|2|>|1|=|\lambda_1|=|\lambda_2|$.

<div class="alert alert-block alert-success">
<p><span class="math inline">\(\lambda_1 =\lambda_2= 1\)</span></p>
</div>

The eigenvectors corresponding to $\lambda_1 =\lambda_2 = 1$:
\begin{align*}
&(\lambda_1 I-A)X =0,
\quad \Rightarrow   \quad
\left(I-\begin{bmatrix} 1 & 1 & 0\\ 0 & 2 & 0\\ 0 & 2 & 1 \end{bmatrix} \right)X =\begin{bmatrix}0\\ 0\\0\end{bmatrix},
\quad \Rightarrow   \quad
\begin{bmatrix}0 & -1 & 0\\ 0 & -1 & 0\\ 0 & -2 & 0 \end{bmatrix}X =\begin{bmatrix}0\\ 0\\0\end{bmatrix}.
\end{align*}
The augmented matrix for finding the solutions is given by
\begin{align*}
\left[\begin{array}{ccc|c} 0 & -1 & 0 & 0\\ 0 & -1 & 0 & 0\\ 0 & -2 & 0 & 0 \end{array}\right]
\end{align*}
and the reduced row-echelon form of this matrix is
\begin{align*}
\left[\begin{array}{ccc|c} 0 & {1} & 0 & 0\\ 0 & 0 & 0 & 0\\ 0 & 0 & 0 & 0 \end{array}\right]
\end{align*}
Hence, the general solution $X$ to $(I-A)X =0$ is
\begin{align*}
s \begin{bmatrix} 1\\ 0\\ 0  \end{bmatrix}+t \begin{bmatrix} 0\\ 0\\ 1  \end{bmatrix},\quad s,t\neq0.
\end{align*}
Therefore, we can use $X_1 =\begin{bmatrix} 1\\ 0\\ 0 \end{bmatrix}$
and $X_2 =\begin{bmatrix} 0\\ 0\\ 1  \end{bmatrix}$ as the basic eigenvectors corresponding to \linebreak $\lambda_1=\lambda_2= 1$.

<div class="alert alert-block alert-success">
<p><span class="math inline">\(\lambda_3= 2\)</span></p>
</div>

Similarly,
\begin{align*}
&(\lambda_3 I-A)X =0,
\quad \Rightarrow   \quad
\left(2I-\begin{bmatrix} 1 & 1 & 0\\ 0 & 2 & 0\\ 0 & 2 & 1  \end{bmatrix} \right)X =\begin{bmatrix}0\\ 0\\0\end{bmatrix},
\quad \Rightarrow   \quad
\begin{bmatrix}1 & -1 & 0\\ 0 & 0 & 0\\ 0 & -2 & 1 \end{bmatrix}X =\begin{bmatrix}0\\ 0\\0\end{bmatrix}.
\end{align*}
The augmented matrix:
\begin{align*}
\left[\begin{array}{ccc|c} 1 & -1 & 0 & 0\\ 0 & 0 & 0 & 0\\ 0 & -2 & 1 & 0 \end{array}\right]
\end{align*}
and the reduced row-echelon form:
\begin{align*}
\left[\begin{array}{ccc|c} {1} & 0 & -\frac{1}{2} & 0\\ 0 & {1} & -\frac{1}{2} & 0\\ 0 & 0 & 0 & 0 \end{array}\right]
\end{align*}
Letting $t=2$, the general solution $X$ to $(4I-A)X =0$ is
\begin{align*}
t \begin{bmatrix} 1/2\\1/2\\1 \end{bmatrix},\quad t\neq0.
\end{align*}
Therefore, we can use $X_3 =\begin{bmatrix} 1\\1\\2 \end{bmatrix}$ as the basic eigenvector corresponding to $\lambda_3 = 2$.

We can construct matrix $P$ as follows.

\begin{align*}
P =\begin{bmatrix}  | & | & |\\  X_1 & X_2 & X_3\\  | & | & |\end{bmatrix}=
\begin{bmatrix}1 & 0 & 1\\ 0 & 0 & 1\\ 0 & 1 & 2 \end{bmatrix}.
\end{align*}
It follows that,

\begin{align*}
P^{-1} =\begin{bmatrix} 1 & -1 & 0\\ 0 & -2 & 1\\ 0 & 1 & 0 \end{bmatrix}.
\end{align*}

Therefore,
\begin{align*}
D=P^{-1}AP=
\begin{bmatrix} 1 & -1 & 0\\ 0 & -2 & 1\\ 0 & 1 & 0 \end{bmatrix}
\begin{bmatrix} 1 & 1 & 0\\ 0 & 2 & 0\\ 0 & 2 & 1 \end{bmatrix}
\begin{bmatrix}1 & 0 & 1\\ 0 & 0 & 1\\ 0 & 1 & 2 \end{bmatrix}
=\begin{bmatrix} 1 & 0 & 0\\ 0 & 1 & 0\\ 0 & 0 & 2 \end{bmatrix}
=\begin{bmatrix} {\color{red}\lambda_1} & 0 & 0\\ 0 & {\color{red}\lambda_2} & 0\\ 0 & 0 & {\color{red}\lambda_3} \end{bmatrix}.
\end{align*}
***

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
<p>Eigenvalues on the main diagonal <u>must</u> be in the same order as the corresponding eigenvectors in <span class="math inline">\(P\)</span>.</p>

</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: 
</b></font>
    
Let $A$ be an $n\times n$ matrix, and suppose that $A$ has distinct eigenvalues $\lambda_1, \lambda_2, \ldots, \lambda_m$. For each $i$, let $X_i$ be a $\lambda_i$-eigenvector of $A$. Then $\{ X_1, X_2, \ldots, X_m\}$ is linearly independent.
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Diagonalizability
</b></font>
    
Determining whether or not a square matrix $A$ is diagonalizable can be done using eigenvalues and eigenvectors of the matrix $A$.
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: 
</b></font>
    
Let $A$ be an $n \times n$ matrix and suppose it has $n$ distinct eigenvalues. Then it follows that $A$ is diagonalizable.
</div>

<font color='Blue'><b>Example</b></font>:
Show that the matrix
\begin{align*}
\left[\begin{array}{ccc} 1 & 2 & 0\\ 1 & 2 & 0\\ 2 & 1 & 2 \end{array}\right]
\end{align*}
is diagonalizable.

<font color='Green'><b>Solution</b></font>:
$A$ has characteristic polynomial
\begin{align*}
c_A(\lambda) =\left|\begin{array}{ccc} \lambda -1 & -2 & 0\\ -1 & \lambda -2 & 0\\ -2 & -1 & \lambda -2 \end{array}\right|=
( \lambda -2 )\left|\begin{array}{cc} \lambda -1 & -2\\ -1 & \lambda -2 \end{array}\right|
=\lambda  ( \lambda -2 )( \lambda -3),
\end{align*}
and thus $A$ has distinct eigenvalues $0, 2$ and $3$. Since $A$ is $3 \times 3$ and has three distinct eigenvalues, $A$ is diagonalizable.
***

<div class="alert alert-block alert-success">
<font size="+1"><b>
Lemma: 
</b></font>
    
Let $A$ be an $n \times n$ matrix $A$. Then $A$ is diagonalizable if and only if for each eigenvalue $\lambda$ of A,
the set of all linearly independent eigenvectors corresponding to $\lambda$ has the same number vectors as the multiplicity of $\lambda$.
</div>

It is possible that a matrix $A$ cannot be diagonalized. In other words, we cannot find an invertible matrix P so that $P^{-1} AP = D$.

<font color='Blue'><b>Example</b></font>:
Let $A =\begin{bmatrix} 1 &  1 \\ 0 & 1 \end{bmatrix}$. If possible, find an invertible matrix $P$ and diagonal matrix $D$ so that $P^{-1} AP = D$ .


<font color='Green'><b>Solution</b></font>:
The characteristic polynomial:
\begin{align*}
c_A (\lambda) &= \det(\lambda I-A)=
\left|\begin{array}{cc} \lambda -1 & -1\\ 0 & \lambda -1 \end{array}\right|
=(\lambda - 1)^2=\lambda ^2-2\,\lambda +1.
\end{align*}
The eigenvalues of $A$ are the the roots of $c_A(\lambda)$:
\begin{align*}
\lambda_1 =\lambda_2= 1 \text{ and }\sigma(A)=\{1\}.
\end{align*}

<div class="alert alert-block alert-success">
<p><span class="math inline">\(\lambda_1 = \lambda_2 = 1\)</span></p>
</div>

Finding the eigenvectors corresponding to $\lambda_1 =\lambda_2= 1$:
\begin{align*}
&(\lambda_1 I-A)X =0,
\quad \Rightarrow   \quad
\left(I-\begin{bmatrix} 1 &  1 \\ 0 & 1 \end{bmatrix} \right)X =\begin{bmatrix}0\\ 0\end{bmatrix},
\quad \Rightarrow   \quad
\begin{bmatrix}0 & -1\\ 0 & 0\end{bmatrix}X =\begin{bmatrix}0\\ 0\end{bmatrix}.
\end{align*}
The augmented matrix for finding the solutions is given by
\begin{align*}
\left[\begin{array}{cc|c} 0 & -1 & 0 \\ 0 & 0 & 0 \end{array}\right]
\quad \Rightarrow \quad \Rightarrow 
\left[\begin{array}{cc|c} 0 & {1} & 0\\ 0 & 0 & 0 \end{array}\right].
\end{align*}
Hence, the general solution $X$ to $(0 I-A)X =0$ is
\begin{align*}
t \begin{bmatrix} 1\\0 \end{bmatrix},\quad t\neq0.
\end{align*}
Therefore, we can only use $X_1 =\begin{bmatrix} 1\\0\end{bmatrix}$ as the basic eigenvector corresponding to $\lambda_1 =\lambda_2= 1$.

We only have found one basic eigenvector corresponding to $\lambda_1 =\lambda_2= 1$, but the multiplicity of $\lambda_1 =\lambda_2=1$ is 2. Therefore
this matrix is \textbf{not} diagonalizable.

The matrix $A$ has one eigenvalue of multiplicity two, but only one basic eigenvector. In order to diagonalize $A$, we need to construct an invertible $2\times 2$ matrix $P$. However, because $A$ only has one basic eigenvector, we cannot construct this $P$. Note that if we were to use $X_1$ as both columns of $P$, $P$ would not be invertible ($\det(P)=0$). For this reason, we cannot repeat eigenvectors in $P$.
***

## 7.2.3 Complex Eigenvalues

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>

Let $z$ denote the conjugate of a complex number $z$. If $A$ is a complex matrix, the conjugate matrix $A$ is defined to be the matrix obtained from $A$ by **conjugating every entry**.
</div>

<font color='Blue'><b>Example</b></font>:
1.  If $A=\begin{bmatrix} 1 & 1+i \\ 2i & 1\end{bmatrix}$, then
    $\bar{A}=\begin{bmatrix} 1 & 1-i \\ -2i & 1\end{bmatrix}$.

2.  If $B=\begin{bmatrix} 1 \\ 1+i \\ -1+i \end{bmatrix}$, then
    $\bar{B}=\begin{bmatrix} 1 \\ 1-i \\ -1-i\end{bmatrix}$.


<font color='Blue'><b>Example</b></font>:
Find the eigenvalues of $A=\left[\begin{array}{ccc} -2 & -2 & -9\\ -1 & 1 & -3\\ 1 & 1 & 4 \end{array}\right]$.


<font color='Green'><b>Solution</b></font>:
\begin{align*}
c_A (\lambda) &= \det(\lambda I-A)
=\left|\begin{array}{ccc} \lambda +2 & 2 & 9\\ 1 & \lambda -1 & 3\\ -1 & -1 & \lambda -4 \end{array}\right|
\\& =\left|\begin{array}{ccc} \lambda +2 & 2 & 9\\ 1 & \lambda -1 & 3\\ 0 & \lambda -2 & \lambda -1 \end{array}\right|
\\& =\left|\begin{array}{ccc} \lambda -1 & 5-3\,\lambda  & 0\\ 1 & \lambda -1 & 3\\ 0 & \lambda -2 & \lambda -1 \end{array}\right|
\\&
=(\lambda -1)\left|\begin{array}{cc} \lambda -1 & 3\\ \lambda -2 & \lambda -1 \end{array}\right|
-(5-3\,\lambda)\left|\begin{array}{cc} 1 & 3\\ 0 & \lambda -1 \end{array}\right|
\\&
=(\lambda -1)(\lambda^2 - 5\lambda + 7)-(5-3\,\lambda)(\lambda - 1)
\\&
=(\lambda -1)\left((\lambda^2 - 5\lambda + 7)-(5-3\,\lambda)\right)
\\&
=(\lambda -1)\left(\lambda^2 - 5\lambda + 7-5+3\,\lambda\right)
\\&
=(\lambda -1)\left(\lambda^2 - 2\lambda + 2\right)
\end{align*}
To find the roots of $c_A (\lambda)$, we set each parts equal to zero that is
\begin{align*}
\begin{cases}
\lambda -1=0,
\\\\
\lambda^2 - 2\lambda + 2=0.
\end{cases}
\quad \Rightarrow \quad
\begin{cases}
\lambda =1,
\\\\
\dfrac{2\pm\sqrt{(-2)^2-4(1)(2)}}{2}=\dfrac{2\pm\sqrt{-4}}{2}=\dfrac{2\pm2i}{2}=1\pm i.
\end{cases}
\end{align*}
Therefore, $\sigma(A)=\{1,1+ i,1- i\}$.
***

<div class="alert alert-block alert-info">
<font size="+1"><b>
Proposition: 
</b></font>
    
Let $A$  be a matrix with \underline{real entries}. If $\lambda$ is a complex eigenvalue with eigenvector $X$, then
$\overline{\lambda}$ is a complex eigenvalue with eigenvector $\overline{X}$.

In other words, both eigenvalues and eigenvectors come in conjugate pairs.
</div>

<font color='Blue'><b>Example</b></font>:
Let $A =  \begin{bmatrix} 1 & 0 & 0\\ 0 & 2 & -1\\ 0 & 1 & 2 \end{bmatrix}$. Find the eigenvalues and eigenvectors of $A$.


<font color='Green'><b>Solution</b></font>:
The characteristic polynomial:
\begin{align*}
c_A (\lambda) &=
\left|\begin{array}{ccc} \lambda -1 & 0 & 0\\ 0 & \lambda -2 & 1\\ 0 & -1 & \lambda -2 \end{array}\right|=
(\lambda - 1)(\lambda^2 - 4\lambda + 5).
\end{align*}
The eigenvalues of $A$ are the the roots of $c_A(\lambda)$:
\begin{align*}
\lambda_1=1,~\lambda_1=2+i\quad \text{and} \quad  \lambda_3 = 2-i.
\end{align*}

<div class="alert alert-block alert-success">
<p><span class="math inline">\(\lambda_1 = 1\)</span></p>
</div>

We have
\begin{align*}
&(\lambda_1 I-A)X =0,
\quad \Rightarrow   \quad
\left(I-\begin{bmatrix} 1 & 0 & 0\\ 0 & 2 & -1\\ 0 & 1 & 2  \end{bmatrix} \right)X =\begin{bmatrix}0\\ 0\\0\end{bmatrix},
\quad \Rightarrow   \quad
\begin{bmatrix}0 & 0 & 0\\ 0 & -1 & 1\\ 0 & -1 & -1 \end{bmatrix}X =\begin{bmatrix}0\\ 0\\0\end{bmatrix}.
\end{align*}
The augmented matrix:
\begin{align*}
\left[\begin{array}{ccc|c} 0 & 0 & 0 & 0\\ 0 & -1 & 1 & 0\\ 0 & -1 & -1 & 0  \end{array}\right]
\quad \Rightarrow{\text{in RREF}}\quad \Rightarrow
\left[\begin{array}{ccc|c} 0 & {1} & 0 & 0\\ 0 & 0 & {1} & 0\\ 0 & 0 & 0 & 0  \end{array}\right]
\end{align*}
The general solution $X$ to $(I-A)X =0$:
\begin{align*}
t \begin{bmatrix} 1\\0\\0 \end{bmatrix},\quad t\neq0.
\end{align*}
Therefore, we can use $X_1=\begin{bmatrix} 1\\0\\0  \end{bmatrix}$ as the basic eigenvector corresponding to $\lambda_1 =1$.

<div class="alert alert-block alert-success">
<p><span class="math inline">\(\lambda_1 = 2 + i\)</span></p>
</div>

We have
\begin{align*}
&(\lambda_2 I-A)X =0,
\quad \Rightarrow   \quad
\left((2+i)I-\begin{bmatrix} 1 & 0 & 0\\ 0 & 2 & -1\\ 0 & 1 & 2   \end{bmatrix} \right)X =\begin{bmatrix}0\\ 0\\0\end{bmatrix},
\quad \Rightarrow   \quad
\begin{bmatrix}1+i & 0 & 0\\ 0 & i & 1\\ 0 & -1 & i \end{bmatrix}X =\begin{bmatrix}0\\ 0\\0\end{bmatrix}.
\end{align*}
The augmented matrix:
\begin{align*}
\left[\begin{array}{ccc|c} 1+i & 0 & 0 & 0\\ 0 & i & 1 & 0\\ 0 & -1 & i & 0  \end{array}\right]
\quad \Rightarrow{\text{in RREF}}\quad \Rightarrow
\left[\begin{array}{ccc|c} {1} & 0 & 0 & 0\\ 0 & {1} & -i & 0\\ 0 & 0 & 0 & 0  \end{array}\right].
\end{align*}
The general solution $X$ to $((2+i)I-A)X =0$:
\begin{align*}
t \begin{bmatrix} 0\\i\\1 \end{bmatrix},\quad t\neq0.
\end{align*}
Thus, we can use $X_2=\begin{bmatrix} 0\\i\\1\end{bmatrix}$ as the basic eigenvector corresponding to $\lambda_2 = 2+i$.

<div class="alert alert-block alert-success">
<p><span class="math inline">\(\lambda_1 = 2 - i\)</span></p>
</div>

Since $2+i$ and $2-i$ are conjugates, the basic eigenvector corresponding $\lambda_3= 2-i$ can be find by applying conjugate on the basic eigenvector of $\lambda_2=2+i$. Hence, the general solution $X$ to $((2+i)I-A)X =0$ is
\begin{align*}
t \begin{bmatrix} 0\\-i\\1 \end{bmatrix},\quad t\neq0.
\end{align*}
Therefore, we can use $X_3=\begin{bmatrix} 0\\-i\\1\end{bmatrix}$ as the basic eigenvector corresponding to $\lambda_3= 2-i$.

This can be easily verified, observe that
\begin{align*}
(\lambda_3 I-A)X_3=\left((2-i)I-\begin{bmatrix} 1 & 0 & 0\\ 0 & 2 & -1\\ 0 & 1 & 2  \end{bmatrix} \right)\begin{bmatrix} 0\\-i\\1\end{bmatrix}=
\begin{bmatrix}1-i & 0 & 0\\ 0 & -i & 1\\ 0 & -1 & -i\end{bmatrix}\begin{bmatrix} 0\\-i\\1\end{bmatrix}=\begin{bmatrix} 0\\0\\0\end{bmatrix}.
\end{align*}

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
