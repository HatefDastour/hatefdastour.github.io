
Diagonalization
==============================

Similarity and Diagonalization
----------------------------------

**Trace of a Matrix**:
The trace of an $n\times n$ matrix $A$ is defined to be the sum of the
main diagonal elements of $A$
\begin{align*}
tr(A) = \sum_{i=1}^{n}a_{ii}.
\end{align*}

<font color='Blue'><b>Example</b></font>:
Find the trace of a matrix of $A=\left[\begin{array}{ccc} 1 & 1 & 2\\ 3 & 4 & 5\\ 1 & 2 & 3 \end{array}\right]$.

<font color='Green'><b>Solution</b></font>:
The trace of $A$:
\begin{align*}
tr(A)=1+4+3=8.
\end{align*}

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: Properties of Trace
</b></font>
    
<p>For <span class="math inline">\(n\times n\)</span> matrices <span class="math inline">\(A\)</span> and <span class="math inline">\(B\)</span>, and any <span class="math inline">\(k \in \mathbb{R}\)</span>,</p>
<ol>
<li><p><span class="math inline">\(tr (A+B) = tr (A)+ tr (B)\)</span>,</p></li>
<li><p><span class="math inline">\(tr (kA) = k\, tr (A)\)</span></p></li>
<li><p><span class="math inline">\(tr (AB) = tr (BA)\)</span></p></li>
</ol>
</div>

**Similar Matrices**:
If $A$ and $B$ be $n\times n$, we say that $A$ and $B$ are similar, and write $A \sim B$, if $B = P^{-1} AP$ for some invertible matrix $P$.

<div class="alert alert-block alert-success">
<font size="+1"><b>
Lemma: Similarity is an Equivalence Relation
</b></font>
    
<p>Similarity is an equivalence relation, i.e. for <span class="math inline">\(n\times n\)</span> matrices <span class="math inline">\(A\)</span>, <span class="math inline">\(B\)</span>, and <span class="math inline">\(C\)</span>,</p>
<ul>
<li><p><span class="math inline">\(A \sim A\)</span>, (reflexive)</p></li>
<li><p>If <span class="math inline">\(A \sim B\)</span>, then <span class="math inline">\(B \sim A\)</span>,(symmetric)</p></li>
<li><p>If <span class="math inline">\(A \sim B\)</span> and <span class="math inline">\(B \sim C\)</span> , then <span class="math inline">\(A \sim C\)</span>,(transitive)</p></li>
</ul>
</div>

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: Properties of Similar Matrices
</b></font>
    
<p>If <span class="math inline">\(A\)</span> and <span class="math inline">\(B\)</span> are <span class="math inline">\(n\times n\)</span> matrices and <span class="math inline">\(A \sim B\)</span>, then</p>
<ul>
<li><p><span class="math inline">\(\det(A)=\det(B)\)</span>,</p></li>
<li><p><span class="math inline">\(rank(A)=rank(B)\)</span>,</p></li>
<li><p><span class="math inline">\(tr (A) = tr (B)\)</span>,</p></li>
<li><p><span class="math inline">\(c_A (\lambda) = c_B (\lambda)\)</span>,(<span class="math inline">\(A\)</span> and <span class="math inline">\(B\)</span> have the same characteristic polynomial).</p></li>
<li><p><span class="math inline">\(\sigma(A)=\sigma(B)\)</span>,(<span class="math inline">\(A\)</span> and <span class="math inline">\(B\)</span> have the same eigenvalues).</p></li>
</ul>
</div>

**Diagonal Matrix**:
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

**Diagonalizable**: 
Let $A$ be an $n\times n$ matrix. Then $A$ is said to be \textbf{diagonalizable} if there exists an invertible matrix $P$
such that $P^{-1} AP = D$ where $D$ is a diagonal matrix.
\\~\\
Here the invertible matrix $P$ is called a \textbf{diagonalizing matrix} for $A$.

<div class="alert alert-block alert-info">
<font size="+1"><b>
Proposition:
</b></font>
    
<p>An <span class="math inline">\(n\times n\)</span> matrix <span class="math inline">\(A\)</span> is <strong>diagonalizable</strong> if <span class="math inline">\(A\sim D\)</span> for some <strong>diagonal matrix</strong> <span class="math inline">\(D\)</span>.</p>

</div>

**Dominant Eigenvalue**: If $\lambda$ is an eigenvalue of $A$ that is larger in absolute value
than any other eigenvalue, it is called the **dominant eigenvalue** of
$A$.

Note that the above equation can be rearranged as $A = PDP^{-1}$ . Suppose we wanted to compute $A^{100}$. By diagonalizing A first it suffices to then compute $\left(PDP^{-1}\right)^{100}$, which reduces to $PD^{100} P^{-1}$. This last computation is much simpler than $A^{100}$.

Diagonalizing a Matrix
------------------------------------

Let $A$ be an $n\times n$ matrix. The process of finding an
**invertible** matrix $P$ and a **diagonal** matrix $D$ so that
$A=PDP^{-1}$ is referred to as **diagonalizing** the matrix $A$, and $P$
is called the **diagonalizing** matrix for $A$.

The key to diagonalizing a matrix (finding the matrices $P$ and $D$)
lies in the eigenvectors and eigenvalues of the matrix $A$.

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: Eigenvectors and Diagonalizable Matrices
</b></font>
    
<p>Let <span class="math inline">\(A\)</span> be an <span class="math inline">\(n\times n\)</span> matrix.</p>
<ol>
<li><p><span class="math inline">\(A\)</span> is diagonalizable if and only if it has eigenvectors <span class="math inline">\(X_1, X_2, \ldots, X_n\)</span> so that <span class="math inline">\(P = \left[\begin{array}{cccc} X_1 &amp; X_2 &amp; \cdots &amp; X_n \end{array}\right]\)</span> is invertible.</p></li>
<li><p>If <span class="math inline">\(P\)</span> is invertible, then <span class="math display">\[P^{-1}AP=\mathrm{Diag}(\lambda_1, \lambda_2, \ldots, \lambda_n )\]</span> where <span class="math inline">\(\lambda_i\)</span> is the eigenvalue of <span class="math inline">\(A\)</span> corresponding to the eigenvector <span class="math inline">\(X_i\)</span>, i.e., <span class="math inline">\(AX_i=\lambda_i X_i\)</span>.</p></li>
</ol>
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
P^{-1} =\begin{bmatrix} 1 & -1 & 0\\ 0 & -2 & 1\\ 0 & 1 & 0
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

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: 
</b></font>
    
<p>Let <span class="math inline">\(A\)</span> be an <span class="math inline">\(n\times n\)</span> matrix, and suppose that <span class="math inline">\(A\)</span> has distinct eigenvalues <span class="math inline">\(\lambda_1, \lambda_2, \ldots, \lambda_m\)</span>. For each <span class="math inline">\(i\)</span>, let <span class="math inline">\(X_i\)</span> be a <span class="math inline">\(\lambda_i\)</span>-eigenvector of <span class="math inline">\(A\)</span>. Then <span class="math inline">\(\{ X_1, X_2, \ldots, X_m\}\)</span> is linearly independent.</p>

</div>

**Diagonalizability**: Determining whether or not a square matrix $A$ is diagonalizable can be done using eigenvalues and eigenvectors of the matrix $A$.

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: 
</b></font>
    
<p>Let <span class="math inline">\(A\)</span> be an <span class="math inline">\(n \times n\)</span> matrix and suppose it has <span class="math inline">\(n\)</span> distinct eigenvalues. Then it follows that <span class="math inline">\(A\)</span> is diagonalizable.</p>

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
    
<p>Let <span class="math inline">\(A\)</span> be an <span class="math inline">\(n \times n\)</span> matrix <span class="math inline">\(A\)</span>. Then <span class="math inline">\(A\)</span> is diagonalizable if and only if for each eigenvalue <span class="math inline">\(\lambda\)</span> of A, the set of all linearly independent eigenvectors corresponding to <span class="math inline">\(\lambda\)</span> has the same number vectors as the multiplicity of <span class="math inline">\(\lambda\)</span>.</p>


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

Complex Eigenvalues
------------------------------

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>

<p>Let <span class="math inline">\(z\)</span> denote the conjugate of a complex number <span class="math inline">\(z\)</span>. If <span class="math inline">\(A\)</span> is a complex matrix, the conjugate matrix <span class="math inline">\(A\)</span> is defined to be the matrix obtained from <span class="math inline">\(A\)</span> by <u>conjugating every entry</u>.</p>


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
    
<p>Let <span class="math inline">\(A\)</span> be a matrix with <u>real entries</u>. If <span class="math inline">\(\lambda\)</span> is a complex eigenvalue with eigenvector <span class="math inline">\(X\)</span>, then <span class="math inline">\(\overline{\lambda}\)</span> is a complex eigenvalue with eigenvector <span class="math inline">\(\overline{X}\)</span>.</p>
<p>In other words, both eigenvalues and eigenvectors come in conjugate pairs.</p>

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
