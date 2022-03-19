Projections
========================

```{image} ../Figures/fig4_15.png
:width: 200px
:align: center
```

If a nonzero vector $\vec{d}$ is specified, the key idea of projection is to be able to write an arbitrary vector $u$ as a sum of two vectors,
\begin{equation*}
\vec{u}=\vec{u}_{\parallel}+\vec{u}_{\perp}.
\end{equation*}
where $\vec{u}_{\parallel}$ is a parallel to $\vec{d}$ , and $\vec{u}_{\perp}=\vec{u}-\vec{u}_{\parallel}$ is perpendicular to $\vec{d}$.

Suppose that $\vec{u}$ and $\vec{d}\neq 0$ emanate from a common tail $Q$. Let $P$ be the tip of $\vec{u}$, and let $P_1$ denote the foot of the perpendicular from $P$ to the line through $Q$ parallel to $\vec{d}$.

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: Vector Projections
</b></font>

<p>Let <span class="math inline">\(\vec{u}\)</span> and <span class="math inline">\(\vec{d}\)</span> be nonzero vectors. Then there exist unique vectors <span class="math inline">\(\vec{u}_{\parallel}\)</span> and <span class="math inline">\(\vec{u}_{\perp}\)</span> such that <span class="math display">\[\vec{u}=\vec{u}_{\parallel}+\vec{u}_{\perp}.\]</span> where <span class="math inline">\(\vec{u}_{\parallel}\)</span> is a scalar multiple of <span class="math inline">\(\vec{d}\)</span> , and <span class="math inline">\(\vec{u}_{\perp}\)</span> is perpendicular to <span class="math inline">\(\vec{d}\)</span>.</p>
    
</div>

**Vector Projection**: Let $\vec{u}$ and $\vec{d}$ be vectors. Then, the projection of $\vec{u}$ onto $\vec{d}$ is given by
\begin{equation*}
\vec{u}_{\parallel}=proj_{\vec{d}}{\vec{u}}=
\left( \frac{\vec{u} \bullet \vec{d}}{\vec{d} \bullet \vec{d}}\right)\vec{d}=
\frac{\vec{u}\bullet\vec{d}}{\|\vec{d}\|^2}\vec{d}.
\end{equation*}

<div class="alert alert-block alert-success">
<font size="+1"><b>
Summary:
</b></font>
<ol>
<li><p><span class="math inline">\(\vec{u}_{\parallel}=\overrightarrow{OP_1}\)</span>.</p></li>
<li><p><span class="math inline">\(\vec{u}_{\parallel}\)</span> is parallel to <span class="math inline">\(\vec{d}\)</span>.</p></li>
<li><p><span class="math inline">\(\vec{u}_{\perp}= u - \vec{u}_{\parallel}\)</span> is orthogonal to <span class="math inline">\(\vec{d}\)</span>. In other words <span class="math display">\[\vec{u}_{\perp}=\vec{u}-\frac{\vec{u}\bullet\vec{d}}{\|\vec{d}\|^2}\vec{d}.\]</span></p></li>
<li><p><span class="math inline">\(\vec{u}=\vec{u}_{\parallel}+\vec{u}_{\perp}\)</span>.</p></li>
</ol>
 
```{image} ../Figures/fig4_15.png
:width: 200px
:align: center
```
</div>

<font color='Blue'><b>Example</b></font>:
Let $\vec{u}=\begin{bmatrix} 2 \\ 1 \end{bmatrix}$ and
$\vec{d}=\begin{bmatrix} 1 \\ 0 \end{bmatrix}$. Find vectors
$\vec{u}_{\parallel}$ and $\vec{u}_{\perp}$ such that,

1.  $\vec{u}=\vec{u}_{\parallel}+\vec{u}_{\perp}$,

2.  $\vec{u}_{\parallel}$ is parallel to $\vec{d}$,

3.  $\vec{u}_{\perp}$ is perpendicular to $\vec{d}$.

<font color='Green'><b>Solution</b></font>:
\begin{align*}
\vec{u}_{\parallel}&=proj_{\vec{d}}{\vec{u}}=\frac{\vec{u}\bullet \vec{d}}{\vec{d}\bullet \vec{d}}\vec{d}
=\frac{\begin{bmatrix} 2 \\ 1 \end{bmatrix} \bullet \begin{bmatrix}1 \\ 0\end{bmatrix}}
{\begin{bmatrix}1 \\ 0\end{bmatrix} \bullet \begin{bmatrix}1 \\ 0\end{bmatrix}}
\begin{bmatrix}1 \\ 0\end{bmatrix}=
\frac{(2)(1)+(1)(0)}{(1)(1)+(0)(0)}\begin{bmatrix}1 \\ 0\end{bmatrix}
=2\begin{bmatrix}1 \\ 0\end{bmatrix}=\begin{bmatrix}2 \\ 0\end{bmatrix},
\\
\vec{u}_{\perp}&= u - \vec{u}_{\parallel}=\begin{bmatrix} 2 \\ 1 \end{bmatrix}-\begin{bmatrix}2 \\ 0\end{bmatrix}=\begin{bmatrix}0 \\ 1\end{bmatrix}.
\end{align*}
We also can verify that $\vec{u}=\vec{u}_{\parallel}+\vec{u}_{\perp}$.

Check https://www.geogebra.org/classic/nqdjwxau for the graph.
***

<font color='Blue'><b>Example</b></font>:
Consider $P=(2,2,-1)$ and the line
\begin{align*}
L:~\begin{cases}\begin{bmatrix}  x \\   y \\   z \end{bmatrix}=
\begin{bmatrix}  1 \\   1 \\   1 \end{bmatrix}+t\begin{bmatrix}  1 \\   -2 \\   1 \end{bmatrix}\end{cases}.
\end{align*}
Find point $Q$ on $L$ closest to $P$.

<font color='Green'><b>Solution</b></font>:
```{image} ../Figures/fig4_17.png
:width: 450px
:align: center
```
     
It can be seen that the direction of $L$ is
$\vec{d}=\begin{bmatrix} 1 & -2 & 1 \end{bmatrix}^T$. Now, consider a
point (any point!) on $L$, for example, $P_0=(1,1,1)$. To find $Q$:

1.  We need $\overrightarrow{P_0P}$ and $\overrightarrow{P_0Q}$:
    \begin{align*}
    \overrightarrow{P_0P}&=
    \begin{bmatrix} 2\\ 2\\ -1 \end{bmatrix}-\begin{bmatrix} 1\\ 1\\ 1  \end{bmatrix}=\begin{bmatrix} 1\\ 1\\ -2\end{bmatrix}
    \\
    \overrightarrow{P_0Q}&=
    \frac{\overrightarrow{P_0P}\bullet \vec{d}}{\vec{d}\bullet \vec{d}}\vec{d}=
    \frac{\begin{bmatrix} 1\\ 1\\ -2 \end{bmatrix}\bullet\begin{bmatrix} 1\\ -2\\ 1 \end{bmatrix}}
    {\begin{bmatrix} 1\\ -2\\ 1 \end{bmatrix}\bullet\begin{bmatrix} 1\\ -2\\ 1 \end{bmatrix}}
    \begin{bmatrix}1\\ -2\\ 1\end{bmatrix}
    =-\frac{1}{2}\begin{bmatrix}1\\ -2\\ 1\end{bmatrix}
    =\begin{bmatrix}-\frac{1}{2}\\ 1\\ -\frac{1}{2}\end{bmatrix}.
	\end{align*}

2.  $Q$ is given by:
	\begin{align*}
    \overrightarrow{0Q}&=\overrightarrow{0P_0}+ \overrightarrow{P_0Q}
    =\begin{bmatrix} 1\\ 1\\ 1\end{bmatrix}-\frac{1}{2}\begin{bmatrix}1\\ -2\\ 1\end{bmatrix}
    =\begin{bmatrix} \frac{1}{2}\\ 2\\ \frac{1}{2}\end{bmatrix}.
	\end{align*}

Hence, $Q=\left(\dfrac{1}{2}, 2, \dfrac{1}{2}\right)$.

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
