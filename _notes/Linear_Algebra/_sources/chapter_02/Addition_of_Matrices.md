# 2.1.1 Addition of Matrices

We can add two matrices only if all matrices in the sum need have the same size.

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Matrix Addition
</b></font>

If $A$ and $B$ are matrices of the same size, their sum $A+B$ is the matrix formed by adding corresponding entries.
</div>

<font color='Blue'><b>Example</b></font>:
Let $A=\begin{bmatrix}  1 & -2 & 4\\ 3 & 0 & 7 \end{bmatrix}$
and $B=\begin{bmatrix}  6 & 2 & 4\\ -2 & 1 & -1 \end{bmatrix}$. Find $A+B$.

<font color='Green'><b>Solution</b></font>:

\begin{align*}
A+B &=\begin{bmatrix}  1 & -2 & 4\\ 3 & 0 & 7 \end{bmatrix}+\begin{bmatrix}  6 & 2 & 4\\ -2 & 1 & -1 \end{bmatrix}
\\ &
=\begin{bmatrix}  1+6 & -2+2 & 4+4\\ 3+(-2) & 0+1 & 7+(-1) \end{bmatrix}
\\ &
=\begin{bmatrix}  7 & 0 & 8\\ 1 & 1 & 6 \end{bmatrix}.
\end{align*}
***

<font color='Blue'><b>Example</b></font>:
If $C=\begin{bmatrix}  1 & -3 & 4\\ 0 & 1 & 2 \end{bmatrix}$
and $D=\begin{bmatrix}  1 & 1\\ 1 & 3 \end{bmatrix}$, we cannot have $C+D$ since $C$ is $2\times 3$ and $D$ is $2\times 2$.

<div class="alert alert-secondary" role="alert">
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
