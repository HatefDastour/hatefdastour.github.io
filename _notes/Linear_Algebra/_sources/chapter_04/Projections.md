# Projections


```{image} ../Figures/fig4_15.png
:width: 200px
:align: center
```

The key idea of projection is writing a vector as a sum of two vectors. For a nonzero vector $\vec{d}$ and an arbitrary vector $\vec{u}$, we have,
\begin{equation*}
\vec{u}=\vec{u}_{\parallel}+\vec{u}_{\perp}.
\end{equation*}
where $\vec{u}_{\parallel}$ is a vector parallel to vector $\vec{d}$ ($\parallel$ here denotes parallel) , and $\vec{u}_{\perp}=\vec{u}-\vec{u}_{\parallel}$ is a vector perpendicular to vector $\vec{d}$ ($\perp$ here shows perpendicular).

Assume that two vectors  $\vec{u}$ and $\vec{d}\neq 0$ ($\vec{d}$ is nonzero) emanate from the same tail (point $Q$). Let point $P$ be the tip of vector  $\vec{u}$, and also $P_1$ denote the foot of the perpendicular from $P$ to the line through $Q$ parallel to $\vec{d}$.

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Vector Projections
</b></font>

For two nonzero vectors $\vec{u}$ and $\vec{d}$, there exist \textbf{unique} vectors $\vec{u}_{\parallel}$ and $\vec{u}_{\perp}$ such that
\begin{equation*}
\vec{u}=\vec{u}_{\parallel}+\vec{u}_{\perp}.
\end{equation*}
where $\vec{u}_{\parallel}$ is parallel to vector $\vec{d}$ (is a scalar multiplied by $\vec{d}$), and $\vec{u}_{\perp}$ is perpendicular to $\vec{d}$.

```{image} ../Figures/fig4_15.png
:width: 200px
:align: center
```
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Vector Projection
</b></font>

The projection of vector $\vec{u}$ onto vector $\vec{d}$, denoted by $\vec{u}_{\parallel}$, is defined as follows
\begin{equation*}
\vec{u}_{\parallel}=proj_{\vec{d}}{\vec{u}}=
\left( \frac{\vec{u} \bullet \vec{d}}{\vec{d} \bullet \vec{d}}\right)\vec{d}=
\frac{\vec{u}\bullet\vec{d}}{\|\vec{d}\|^2}\vec{d}.
\end{equation*}
</div>

<div class="alert alert-block alert-success">
<font size="+1"><b>
Summary:
</b></font>

* $\vec{u}_{\parallel}=\overrightarrow{OP_1}$.
* $\vec{u}_{\parallel}$ is parallel to $\vec{d}$, and
\begin{equation*}
\vec{u}_{\parallel}=proj_{\vec{d}}{\vec{u}}=
\left( \frac{\vec{u} \bullet \vec{d}}{\vec{d} \bullet \vec{d}}\right)\vec{d}=
\frac{\vec{u}\bullet\vec{d}}{\|\vec{d}\|^2}\vec{d}.
\end{equation*}
* $\vec{u}_{\perp}= u - \vec{u}_{\parallel}$ is orthogonal to $\vec{d}$. In other words
\begin{equation*}
\vec{u}_{\perp}=\vec{u}-\frac{\vec{u}\bullet\vec{d}}{\|\vec{d}\|^2}\vec{d}.
\end{equation*}
* $\vec{u}=\vec{u}_{\parallel}+\vec{u}_{\perp}$. 

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

<center>
<iframe src="https://www.geogebra.org/classic/p7wqv39m?embed" width="600" height="400" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>
</center>

<font color='Blue'><b>Example</b></font>:
Consider $P=(2,2,-1)$ and the line
\begin{align*}
L:~\begin{cases}\begin{bmatrix}  x \\   y \\   z \end{bmatrix}=
\begin{bmatrix}  1 \\   1 \\   1 \end{bmatrix}+t\begin{bmatrix}  1 \\   -2 \\   1 \end{bmatrix}\end{cases}.
\end{align*}
Find point $Q$ on $L$ closest to $P$.

<font color='Green'><b>Solution</b></font>:
```{image} ../Figures/fig4_17.png
:width: 340px
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
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
