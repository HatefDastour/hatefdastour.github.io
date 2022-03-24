# 2.1.7 Elementary Matrices

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Elementary Matrices and Row Operations
</b></font>

An $n\times n$ matrix $E$ is an **elementary matrix** if it can be obtained from the identity matrix $I_n$ through a **single row operation** (i.e.  switching the two rows, multiplying a row by some number and adding to another row, etc.). Those which involve switching rows of the identity matrix are called **permutation matrices**.
</div>



For example, the matrix
\begin{align*}
E=\begin{bmatrix}
    1 & 0 & 0 \\
    0 & 0 & 1 \\
    0 & 1 & 0
  \end{bmatrix}
\end{align*}

is the elementary matrix obtained from **switching the last two rows** of $I_{3}$. The matrix
\begin{align*}
E=\begin{bmatrix}
    3 & 0 & 0 \\
    0 & 1 & 0 \\
    0 & 0 & 1
  \end{bmatrix}
\end{align*}
is the elementary matrix obtained from **multiplying the first row** of $I_{3}$ by 3. The matrix
\begin{align*}
E=\begin{bmatrix}
    1 & 0 \\
    5 & 1 \\
  \end{bmatrix}
\end{align*}
is the elementary matrix obtained from **adding $5$ times the first row to the second row** of $I_{2}$.

<div class="alert alert-block alert-success">
    
<li><strong>Multiplication by an Elementary Matrix and Row Operations</strong>:<br />
To perform any of the row operations on a matrix <span class="math inline">\(A\)</span> it suffices to take the product <span class="math inline">\(EA\)</span>, where <span class="math inline">\(E\)</span> is the elementary matrix obtained by using the desired row operation on the identity matrix.</p></li>
<li><strong>Action of Permutation Matrix</strong>:<br />
Let <span class="math inline">\(P^{ij}\)</span> denote the elementary matrix which involves switching the <span class="math inline">\(i^{\text{th}}\)</span> and the <span class="math inline">\(j^{\text{th}}\)</span> rows. Then <span class="math inline">\(P^{ij}\)</span> is a permutation matrix and <span class="math inline">\(P^{ij}A = B\)</span> where <span class="math inline">\(B\)</span> is obtained from <span class="math inline">\(A\)</span> by switching the <span class="math inline">\(i^{\text{th}}\)</span> and the <span class="math inline">\(j^{\text{th}}\)</span> rows.</p></li>
</ul>
    
</div>

<font color='Blue'><b>Example</b></font>:
Let $$P^{23}=\begin{bmatrix}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0 \\
\end{bmatrix},
~A=\begin{bmatrix}
1 & 2 \\
3 & 4 \\
5 & 6
\end{bmatrix}.$$ Find $B$ where $B = P^{23}A$

<font color='Green'><b>Solution</b></font>:
$B$ can be obtained from switching the last two rows of matrix $A$. Therefore,
\begin{align*}
B=\begin{bmatrix}1 & 2 \\
5 & 6 \\
3 & 4
\end{bmatrix}
\end{align*}
***

<div class="alert alert-block alert-success">
    
<ul>
<li><p><strong>Multiplication by a Scalar and Elementary Matrices</strong>:<br />
Let <span class="math inline">\(E(k,i)\)</span> denote the elementary matrix corresponding to the row operation in which the <span class="math inline">\(i^{\text{th}}\)</span> row is multiplied by the nonzero scalar, <span class="math inline">\(k\)</span>. Then <span class="math display">\[E(k,i)A = B\]</span> where <span class="math inline">\(B\)</span> is obtained from <span class="math inline">\(A\)</span> by multiplying the <span class="math inline">\(i^{\text{th}}\)</span> row of <span class="math inline">\(A\)</span> by <span class="math inline">\(k\)</span>.</p></li>
<li><p><strong>Action of Permutation Matrix</strong>:<br />
Let <span class="math inline">\(E(k\times \, i+ \, j)\)</span> denote the elementary matrix obtained from <span class="math inline">\(I\)</span> by adding <span class="math inline">\(k\)</span> times the <span class="math inline">\(i^{\text{th}}\)</span> row to the <span class="math inline">\(j^{\text{th}}\)</span> . Then <span class="math inline">\(E(k\times \, i+ \, j) A = B\)</span> where <span class="math inline">\(B\)</span> is obtained from <span class="math inline">\(A\)</span> by adding <span class="math inline">\(k\)</span> times the <span class="math inline">\(i^{\text{th}}\)</span> row to the <span class="math inline">\(j^{\text{th}}\)</span> row of A.</p></li>
</ul>
    
</div>

<font color='Blue'><b>Example</b></font>:
Let
\begin{align*}
A=\begin{bmatrix}
1 & 2 \\
3 & 4 \\
5 & 6
\end{bmatrix}.
\end{align*}
Find $B = E(3,1)A$ and $C = E(4\times \, 2+ \, 3)A$

<font color='Green'><b>Solution</b></font>:
$B$ can be obtained from multiplying the first row of matrix $A$ by 3 and replacing it with the first row of $A$. Therefore,
$B=\begin{bmatrix}3 & 6 \\3 & 4 \\5 & 6\end{bmatrix}$.

Moreover, $C$ can be obtained from multiplying the second row of matrix $A$ by 4 and adding it to the last row of $A$. Therefore,
$C=\begin{bmatrix}1 & 2 \\3 & 4 \\17 & 22\end{bmatrix}$.
***

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: Elementary Matrices and Inverses
</b></font>
    
Every elementary matrix is invertible and its inverse is also an elementary matrix.
    
</div>

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
