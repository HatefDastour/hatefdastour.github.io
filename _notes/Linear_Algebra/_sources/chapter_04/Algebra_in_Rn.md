# Algebra in $\mathbb{R}^n$

**Addition of Vectors in $\mathbb{R}^n$**:
If $\vec{u}=\begin{bmatrix}u_1 & u_2 & \dots & u_n\end{bmatrix}^T ,~\vec{v}=\begin{bmatrix}v_1 & v_2 & \dots & v_n\end{bmatrix}^T  \in \mathbb{R}^n$ hen $\vec{u}+\vec{v}\in \mathbb{R}^n$ and is defined by
\begin{align*}
\vec{u}+\vec{v}=\begin{bmatrix}u_1\\u_2\\\vdots\\u_n\end{bmatrix}+\begin{bmatrix}v_1\\v_2\\\vdots\\v_n\end{bmatrix}=
\begin{bmatrix}u_1+v_1\\u_2+v_2\\\vdots\\u_n+v_n\end{bmatrix}.
\end{align*}

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: Properties of Vector Addition
</b></font>
    
<p>Let <span class="math inline">\(\vec{u}\)</span>,<span class="math inline">\(\vec{v}\)</span> and <span class="math inline">\(\vec{w}\)</span> be vectors in <span class="math inline">\(\mathbb{R}^n\)</span>. Then, the following properties hold. <span class="math display">\[\begin{array}{llc}
\bullet &\text{The Commutative Law of Addition:} & \vec{u}+\vec{v} = \vec{v}+\vec{u}, \\
\bullet &\text{The Associative Law of Addition:} & ((\vec{u}+\vec{v})+\vec{w} = \vec{u}+(\vec{v}+\vec{w}), \\
\bullet &\text{The Existence of an Additive Identity:} & \vec{u}+0 = \vec{u},\\
\bullet &\text{The Existence of an Additive Inverse:} & \vec{u}+(-\vec{u}) = 0.
\end{array}\]</span></p>
</div>

<font color='Blue'><b>Example</b></font>: If $\vec{u}=\left[\begin{array}{c} 1\\ 2\\ 0\\ 5\\ 6 \end{array}\right]$ and $\vec{v}=\left[\begin{array}{c} 0\\ 2\\ 1\\ 3\\ 7 \end{array}\right]$. Evaluate $\vec{u}+\vec{v}$ and $\vec{u}-\vec{v}$.
***
<font color='Green'><b>Solution</b></font>:
\begin{align*}
\vec{u}+\vec{v}=\left[\begin{array}{c} 1+0\\ 2+2\\ 0+1\\ 5+3\\ 6+7 \end{array}\right]
=\left[\begin{array}{c} 1\\ 4\\ 1\\ 8\\ 13 \end{array}\right],\quad
\vec{u}-\vec{v}=\left[\begin{array}{c} 1-0\\ 2-2\\ 0-1\\ 5-3\\ 6-7 \end{array}\right]
=\left[\begin{array}{c} 1\\ 0\\ -1\\ 2\\ -1 \end{array}\right].
\end{align*}
***

**Scalar Multiplication of Vectors in $\mathbb{R}^n$**: If $\vec{u}=\begin{bmatrix}u_1\\u_2\\\vdots\\u_n\end{bmatrix}$ and $k\in \mathbb{R}$ is a scalar, then $k \vec{u} \in \mathbb{R}^n$ is defined by
\begin{align*}
k\vec{u}=k\,\begin{bmatrix}u_1\\u_2\\\vdots\\u_n\end{bmatrix}=\begin{bmatrix}ku_1\\ku_2\\\vdots\\ku_n\end{bmatrix}.
\end{align*}

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: Properties of Scalar Multiplication
</b></font>
    
<p>The following properties hold for vectors <span class="math inline">\(\vec{u},~\vec{v} \in \mathbb{R}^n\)</span> and <span class="math inline">\(k,~p\)</span> scalars. <span class="math display">\[\begin{array}{llc}
\bullet &\text{The Distributive Law over Vector Addition} & k(\vec{u}+\vec{v}) = k\vec{u}+k\vec{v}, \\
\bullet &\text{The Distributive Law over Scalar Addition:} & (k+ p)\vec{u} = k\vec{u}+ p\vec{u}, \\
\bullet &\text{The Associative Law for Scalar Multiplication:} & k(p\vec{u}) = (kp)\vec{u},\\
\bullet &\text{Rule for Multiplication by 1:} & 1\vec{u} =\vec{u}.
\end{array}\]</span></p>
</div>

**Linear Combination**: A vector $\vec{v}$ is said to be a linear combination of the vectors $\vec{u}_1,\ldots,\vec{u}_n$ if there exist scalars, $a_1,\ldots,a_n$ such that
$$v = a_1 \vec{u}_1 +\ldots+a_n \vec{u}_n$$

<font color='Blue'><b>Example</b></font>:
For example, $\vec{v}=\begin{bmatrix}1 & 2 & 3 & 4\end{bmatrix}^T$ is a linear combination of
$\vec{u}_{1}=\begin{bmatrix}1& 1& 0& 0 \end{bmatrix}^{T}$, $\vec{u}_{2}=\begin{bmatrix}0& 2& 4& 6\end{bmatrix}^{T}$ and
$\vec{u}_{3}=\begin{bmatrix}0& 0& 3& 3\end{bmatrix}^{T}$ since
\begin{align*}
\begin{bmatrix}1\\2\\3\\4\end{bmatrix}=
\begin{bmatrix}1\\ 1\\ 0\\ 0 \end{bmatrix}
+\frac{1}{2}\begin{bmatrix}0\\ 2\\ 4\\ 6\end{bmatrix}
+\frac{1}{3}\begin{bmatrix}0\\ 0\\ 3\\ 3\end{bmatrix}.
\end{align*}

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
