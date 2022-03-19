# Linearly Independent Set of Vectors

**Linear Independence in $\mathbb{R}^n$**:
We call a set $\{ \vec{u}_1 ,~\vec{u}_2, \ldots,~\vec{u}_k\}$ of vectors \textbf{linearly independent} if
\begin{align*}
a_1 \vec{u}_1 +a_2\vec{u}_2 +\ldots+ a_k \vec{u}_k = 0
\end{align*}
then $a_1 =a_2 = \ldots =a_k = 0.$

<div class="alert alert-block alert-success">
<p><strong>Independence Test</strong>:<br />
To verify that a set <span class="math inline">\(\{ \vec{u}_1 ,~\vec{u}_2, \ldots,~\vec{u}_k\}\)</span> of vectors in <span class="math inline">\(\mathbb{R}^n\)</span> is linearly independent, proceed as follows:</p>
<ol>
<li><p>Set a linear combination equal to zero: <span class="math inline">\(a_1 \vec{u}_1 +a_2\vec{u}_2 +\ldots+ a_k \vec{u}_k = 0\)</span>.</p></li>
<li><p>Show that <span class="math inline">\(a_1 =a_2 = \ldots =a_k = 0.\)</span> (that is, the linear combination is trivial).</p></li>
</ol>
<p>Of course, if some nontrivial linear combination vanishes, the vectors are not linearly independent (linearly dependent).</p>
    
</div>

<font color='Blue'><b>Example</b></font>:
Determine whether $\left\{\begin{bmatrix}1\\ 0\\ -2\\ 5\end{bmatrix}, \begin{bmatrix} 2\\ 1\\ 0\\ -1 \end{bmatrix}, \begin{bmatrix} 1\\ 1\\ 2\\ 1 \end{bmatrix}\right\}$ is linearly independent in $\mathbb{R}^4$.

<font color='Green'><b>Solution</b></font>: 
Set $\vec{u}_1=\begin{bmatrix}1\\ 0\\ -2\\ 5\end{bmatrix}$, $\vec{u}_2=\begin{bmatrix} 2\\ 1\\ 0\\ -1 \end{bmatrix}$ and $\vec{u}_3=\begin{bmatrix} 1\\ 1\\ 2\\ 1 \end{bmatrix}$. Then if
\begin{align*}
a_1 \vec{u}_1 +a_2\vec{u}_2 +a_3 \vec{u}_3 = 0,
\end{align*}
we need to show that $a_1 =a_2 = a_3 = 0$.

We have
\begin{align*}
a_1 \begin{bmatrix}1\\ 0\\ -2\\ 5\end{bmatrix} +a_2 \begin{bmatrix} 2\\ 1\\ 0\\ -1 \end{bmatrix} +a_3 \begin{bmatrix} 1\\ 1\\ 2\\ 1 \end{bmatrix}= \begin{bmatrix} 0\\ 0\\ 0\\ 0 \end{bmatrix}.
\end{align*}

This can be represented as the following homogenous linear system
\begin{align*}
\begin{bmatrix}1 & 2 & 1\\ 0 & 1 & 1\\ -2 & 0 & 2\\ 5 & -1 & 1\end{bmatrix}
\begin{bmatrix}a_{1}\\ a_{2}\\ a_{3}\end{bmatrix}
=\begin{bmatrix} 0\\ 0\\ 0\\ 0 \end{bmatrix}.
\end{align*}
The corresponding augmented matrix is given by
\begin{align*}
\left[\begin{array}{ccc|c} 1 & 2 & 1 & 0\\ 0 & 1 & 1 & 0\\ -2 & 0 & 2 & 0\\ 5 & -1 & 1 & 0 \end{array}\right]
\end{align*}
and the reduced row-echelon form of this matrix is
\begin{align*}
\left[\begin{array}{ccc|c} {1} & 0 & 0 & 0\\ 0 & {1} & 0 & 0\\ 0 & 0 & {1} & 0\\ 0 & 0 & 0 & 0 \end{array}\right].
\end{align*}
This means that $a_1=a_2=a_3=0$. Therefore,  these vectors are linearly independent.

<div class="alert alert-block alert-success">
<font size="+1"><b>
Lemma:
</b></font>

<p>A set of <span class="math inline">\(n\)</span> vectors of length <span class="math inline">\(n\)</span> (a set of <span class="math inline">\(n\)</span> vectors in <span class="math inline">\(\mathbb{R}^n\)</span>) is linearly independent if the matrix with these vectors as columns has a <u>non-zero determinant</u>. The set is of course linearly dependent if the determinant is zero.</p>
 
</div>

<font color='Blue'><b>Example</b></font>:
1.  The set of vectors
    $\left\{\begin{bmatrix}1 \\ 1 \\ 2\end{bmatrix}, \begin{bmatrix} 2 \\ 2 \\ 4\end{bmatrix}, \begin{bmatrix}1 \\ 1 \\ 1\end{bmatrix}\right\}$
    is **not** linearly independent since $$\begin{aligned}
    \left|\begin{array}{ccc}1 & 2 & 1\\ 1 & 2 & 1\\ 2 & 4 & 1 \end{array}\right|=0.\end{aligned}$$

2.  The set of vectors
    $\left\{\begin{bmatrix}1 \\ 1 \\ 2\end{bmatrix}, \begin{bmatrix} 0 \\ 2 \\ 1\end{bmatrix}, \begin{bmatrix}1 \\ 1 \\ 1\end{bmatrix}\right\}$
    is linearly independent since $$\begin{aligned}
    \left|\begin{array}{ccc}1 & 0 & 1\\ 1 & 2 & 1\\ 2 & 1 & 1 \end{array}\right|-2\neq 0.\end{aligned}$$

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
