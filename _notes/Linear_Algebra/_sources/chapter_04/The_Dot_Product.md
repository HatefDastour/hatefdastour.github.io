# 4.6 The Dot Product

## Dot Product
<div class="alert alert-info" role="alert">
<font size="+1"><b>
Dot Product
</b></font>

Let $\vec{u}=\begin{bmatrix} u_1 & \dots & u_n \end{bmatrix}^T$, $\vec{v}=\begin{bmatrix} v_1 & \dots & v_n \end{bmatrix}^T$ be two vectors in $\mathbb{R}^n$.
Then, their dot product $\vec{u} \bullet \vec{v}$ is a number defined as
\begin{align*}
\vec{u} \bullet \vec{v}=\begin{bmatrix} u_1 \\ \vdots \\ u_n \end{bmatrix} \bullet \begin{bmatrix} v_1 \\ \vdots \\ v_n \end{bmatrix}=u_1v_1+u_2v_2+\ldots+u_nv_n.
\end{align*}
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
The dot product is also called the **scalar product** and sometimes **inner product**.   
</div>

<font color='Blue'><b>Example</b></font>:
Find $\vec{u} \bullet \vec{v}$ if $\vec{u} =\begin{bmatrix} 3 & 13 & 3 \end{bmatrix}^T$ and $\vec{v} =\begin{bmatrix} 17 & 0 & -1 \end{bmatrix}^T$.
$\vec{d} =\begin{bmatrix} 2 & 2 & 1 \end{bmatrix}^T$.

<font color='Green'><b>Solution</b></font>:
$\vec{u} \bullet \vec{v}= \begin{bmatrix} 3 \\ 13 \\ 3 \end{bmatrix} \bullet \begin{bmatrix} 17 \\ 0 \\ -1 \end{bmatrix}=(3)(17)+(13)(0)+(3)(-1)=48.$
***

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Properties of the Dot Product
</b></font>
    
Let $k$ and $p$ denote scalars and $\vec{u}$, $\vec{v}$, $\vec{w}$ denote vectors. Then the dot product $\vec{u} \bullet \vec{v}$ satisfies the following properties.

* $\vec{u} \bullet \vec{v}= \vec{v} \bullet \vec{u}$,
* $\vec{u} \bullet \vec{u} \geq 0$,
* $\vec{u} \bullet \vec{u}=0$ if and only if $\vec{u} = \vec{0}$,
* $(k\vec{u}+ p\vec{v}) \bullet \vec{w} = k(\vec{u}\bullet \vec{w})+ p(\vec{v}\bullet \vec{w})$,
* $\vec{u}\bullet (k\vec{v}+ p \vec{w}) = k(\vec{u}\bullet \vec{v})+ p(\vec{u}\bullet \vec{w})$,
* $\|\vec{u}\|^2=\vec{u} \bullet \vec{u}$.
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
From the above Theorem, we have $\|\vec{u}\|^2=\vec{u} \bullet \vec{u}$. Therefore, the length of vector $\vec{u}$ can also be found using
\begin{equation*}
\|\vec{u}\|=\sqrt{\vec{u} \bullet \vec{u}}.
\end{equation*}  
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Triangle Inequality
</b></font>
    
For $\vec{v}$, $\vec{w} \in \mathbb{R}^n$
\begin{align*}\|\vec{v}+\vec{w}\| \leq \|\vec{v}\|+\|\vec{w}\|\end{align*}

```{image} ../Figures/fig4_11.png
:width: 300px
:align: center
```
and equality holds if and only if one of the vectors is a non-negative scalar multiple of the other.

Furthermore,
\begin{align*}\|\|\vec{v}\|-\|\vec{w}\|\| \leq \|\vec{v}-\vec{w}\|.\end{align*}  
</div>

## The Included Angle
<div class="alert alert-info" role="alert">
<font size="+1"><b>
The Included Angle
</b></font>

For two vectors $\vec{u}$ and $\vec{v}$, the ***included angle*** is the angle between these two vectors and is given by $\theta$ such that $0 \leq \theta \leq \pi$.
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: The Dot Product and the Included Angle
</b></font>
    
<p>Let <span class="math inline">\(\vec{u}\)</span> and <span class="math inline">\(\vec{v}\)</span> be two vectors in <span class="math inline">\(\mathbb{R}^n\)</span> , and let <span class="math inline">\(\theta\)</span> be the included angle. Then the following equation holds, <span class="math display">\[\begin{aligned}
\vec{u} \bullet \vec{v}=\|\vec{u}\| \|\vec{v}\|\cos(\theta).\end{aligned}\]</span></p>
    
</div>

<font color='Blue'><b>Example</b></font>:
Find the angle between $\vec{u}=\begin{bmatrix}1 \\ 0\end{bmatrix}$ and $\vec{v}=\begin{bmatrix}1 \\ 1\end{bmatrix}$.

<font color='Green'><b>Solution</b></font>:
From the above theorem,
\begin{equation*}
\cos(\theta)=\frac{(1)(1)+(0)(1)}{\sqrt{1^2+0^2}\sqrt{1^2+1^2}}
=\frac{1+0}{\sqrt{1}\sqrt{2}}
=\frac{1}{\sqrt{2}}=\frac{\sqrt{2}}{2}.
\end{equation*}
Therefore, $\theta=\pi/4$.
***

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Perpendicular Vectors
</b></font>
    
<p>Let <span class="math inline">\(\vec{u}\)</span> and <span class="math inline">\(\vec{v}\)</span> be nonzero vectors in <span class="math inline">\(\mathbb{R}^n\)</span>. Then, <span class="math inline">\(\vec{u}\)</span> and <span class="math inline">\(\vec{v}\)</span> are said to be perpendicular exactly when <span class="math display">\[\vec{u} \bullet \vec{v}=0.\]</span></p>
    
</div>

<font color='Blue'><b>Example</b></font>:
Consider the triangle $ABC$ with vertices $A=(1,1,-1)$, $B=(2,3,0)$ and \linebreak $C=(1,0,3)$. Is $ABC$ a right triangle?

<font color='Green'><b>Solution</b></font>:
```{image} ../Figures/fig4_13.png
:width: 300px
:align: center
```

First, let's evaluate $\overrightarrow{AB}$, $\overrightarrow{AC}$ and $\overrightarrow{BC}$.
\begin{align*}
\overrightarrow{AB}=\overrightarrow{OB}-\overrightarrow{OA}=\begin{bmatrix}1\\ 2\\ 1 \end{bmatrix},~
\overrightarrow{BC}=\overrightarrow{OC}-\overrightarrow{OB}=\begin{bmatrix}-1\\ -3\\ 3 \end{bmatrix},~
\overrightarrow{AC}=\overrightarrow{OC}-\overrightarrow{OA}=\begin{bmatrix}0\\ -1\\ 4 \end{bmatrix}.
\end{align*}

$\overrightarrow{AB}$ and $\overrightarrow{AC}$ are perpendicular if $\overrightarrow{AB}\bullet\overrightarrow{AC}=0$. Thus, to have $\overset{\triangle}{ABC}$ as a right triangle, we need to have one of the following dot products zero. However,

Therefore,
\begin{align*}
&\overrightarrow{AB}\bullet \overrightarrow{BC}=\begin{bmatrix}1\\ 2\\ 1 \end{bmatrix} \bullet \begin{bmatrix}-1\\ -3\\ 3 \end{bmatrix}=-4\neq 0,
&\overrightarrow{BC}\bullet \overrightarrow{AC}=\begin{bmatrix}-1\\ -3\\ 3 \end{bmatrix} \bullet\begin{bmatrix}0\\ -1\\ 4 \end{bmatrix}=15\neq 0,
\\
&\overrightarrow{AB}\bullet\overrightarrow{AC}=\begin{bmatrix}1\\ 2\\ 1 \end{bmatrix} \bullet\begin{bmatrix}0\\ -1\\ 4 \end{bmatrix}=2\neq 0&.
\end{align*}
Therefore, $\overset{\triangle}{ABC}$ is not a right triangle.
***

<font color='Blue'><b>Example</b></font>:
Find the shortest distance from $P=(3,2,-1)$ to the line
\begin{align*}
L:\quad \begin{bmatrix} x \\ y \\ z \end{bmatrix}=
\begin{bmatrix} 2 \\ 1 \\ 3 \end{bmatrix}+t\begin{bmatrix} 2 \\ -1 \\ -2 \end{bmatrix}.
\quad, t \in \mathbb{R}.
\end{align*}
Moreover, find the point $Q$ on $L$ that is closest to $P$.

<font color='Green'><b>Solution</b></font>:
```{image} ../Figures/fig4_14.png
:width: 380px
:align: center
```

The shortest distance from a point $P$ to a line $L$ always makes a right angle. Here, we have $\vec{d}=\begin{bmatrix}2&-1&-2\end{bmatrix}^T$ and $P=(3,2,-1)$. We need to find the point $Q$ on $L$ that is closest to $P$. We do not know the point $Q$; however, we know that $Q$ is on $L$. Therefore,

\begin{align*}
Q=(2+2t_0,1-t_0,3-2t_0),\quad \text{for some }t_0\in \mathbb{R}.
\end{align*}
As a result,
\begin{align*}
\overrightarrow{PQ}=\begin{bmatrix}2+2t_0-3\\1-t_0-2\\3-2t_0+1\end{bmatrix}=\begin{bmatrix}-1+2t_0\\-1-t_0\\4-2t_0\end{bmatrix}
\end{align*}
Since $\overrightarrow{PQ}$  and $\vec{d}$ are perpendicular (the angle between $\overrightarrow{PQ}$ and $\vec{d}$ is the right angle),
\begin{align*}
\overrightarrow{PQ}\bullet\vec{d}=0.
\end{align*}
It follows that,
\begin{align*}(-1+2t_0)(2)+(-1-t_0)(-1)+(4-2t_0)(-2)=0. \quad \mathbb{R}ightarrow \quad 9\,t_{0}-9=0.\end{align*}
Hence, $t_0=1$. As a result,
\begin{align*}Q=(2+2(1),1-1,3-2(1))=\left(4, 0, 1\right),\end{align*}
and
\begin{align*}
\|\overrightarrow{PQ}\|=
\sqrt{\left((-1+2(1))^2+(-1-1)^2+(4-2(1))^2\right)^2}
=\sqrt{\left(1+4+4\right)^2}=\sqrt{9}=3.
\end{align*}

Check  for the graph.


<div class="alert alert-danger" role="alert">
<p>Check out <a href="https://www.geogebra.org/3d/ewdr2y6z" target="_blank" rel="noopener noreferrer">https://www.geogebra.org/3d/ewdr2y6z</a> for the graph.

</div>

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
