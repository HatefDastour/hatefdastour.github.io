# Vectors in $\mathbb{R}^n$

-   A scalar quantity has only magnitude. Examples: time, temp, distance, speed,...

-   A vector quantity has both magnitude and direction. Examples: displacement, velocity, force,...

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Ordered n-tuple
</b></font>

An ordered sequence $(a_1 , a_2 , \ldots, a_n )$ of real numbers is an **ordered n-tuple**. Two ordered n-tuple are equal if and only if corresponding entries are the same. In other words,

\begin{align*}
(a_1 , a_2 , \ldots, a_n ) = (b_1 , b_2 , \ldots, b_n )
\end{align*}
if and only if
\begin{align*}
a_1 = b_1 , a_2 = b_2 , \ldots,\text{ and }a_n = b_n
\end{align*}
</div>

The notation $\mathbb{R}^n$ refers to a collection of ordered lists of $n$ real numbers, that is
\begin{align*}
\mathbb{R}^n =\left\{ (x_1,\ldots,x_n ):~x_j \in \mathbb{R}~\text{for}~j = 1,\ldots ,n\right\}.
\end{align*}

In particular, for various values of $n$ we have,
- $n=1$: $\mathbb{R}=\mathbb{R}^1 =\left\{x_1:~x_1 \in \mathbb{R}\right\}$. Examples: $1$, $\sqrt{2}$, $\frac{3}{2}$,...are points in $\mathbb{R}$.

-   $n=2$: $\mathbb{R}^2 =\left\{ (x_1,x_2 ):~x_1,x_2 \in \mathbb{R}\right\}$. Examples: $(1,2)$, $(\sqrt{2},2)$, $\left(\frac{3}{2},0\right)$,...are points in $\mathbb{R}^2.$

-   $n=3$: $\mathbb{R}^3 =\left\{ (x_1,x_2,x_3 ):~x_1,x_2,x_3 \in \mathbb{R}\right\}$. Examples: $(1,2,3)$, $(\sqrt{2},2,1)$, $\left(\frac{3}{2},0,\sqrt{5}\right)$,...are points in $\mathbb{R}^3$.

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Vectors in <span class="math inline">\(\mathbb{R}^n\)</span>
</b></font>

If $\mathbb{R}^n =\left\{ (x_1,\ldots,x_n ):~x_j \in \mathbb{R}~\text{for}~j = 1,\ldots ,n\right\}$, then
\begin{align*}
\vec{x}=\begin{bmatrix} x_1\\ \vdots \\ x_n \\  \end{bmatrix}
\quad \text{or} \quad
\vec{x}=\begin{bmatrix} x_1 & \dots & x_n &  \end{bmatrix}^T
\end{align*}
is called a **vector**.

Each number $x_j$ from vector $\vec{x}$ is called the **components** of $\vec{x}$. Vectors have both size (magnitude) and direction. 
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
* Vectors can be written in either **column vector** form or \textbf{row vector} form
\begin{align*}
\vec{u}&=\begin{bmatrix}    u_1\\ \vdots \\ u_n \\  \end{bmatrix},& {\color{blue}(\text{column vector})}\\
\vec{u}&=\begin{bmatrix}    u_1 & \dots & u_n \\  \end{bmatrix}.& {\color{blue}(\text{row vector})}
\end{align*}
*  Sometimes a **column vector** in $\mathbb{R}^n$ is written in forms of $\begin{bmatrix}    u_1 & \dots & u_n \\  \end{bmatrix}^T$.
</div>


<div class="alert alert-info" role="alert">
<font size="+1"><b>
The Origin
</b></font>

The origin is a point given by $0 = (0,\ldots ,0)$.
</div>


<div class="alert alert-info" role="alert">
<font size="+1"><b>
The Position Vector
</b></font>

A vector that represents the position of a point in a space with respect to the origin is called the position vector. Let $P = (p_1 ,\ldots,p_n )$ be the coordinates of a point in $\mathbb{R}^n$ . Then the vector $\overrightarrow{0P}$  with its tail at $0 =(0,\ldots ,0)$ (the origin) and its tip at $P$ is called the position vector of the point $P$. We write
\begin{align*}
\overrightarrow{0P}=\begin{bmatrix}p_1\\p_2\\\vdots\\p_n\end{bmatrix}-\begin{bmatrix}0\\0\\\vdots\\0\end{bmatrix}
=\begin{bmatrix}p_1-0\\p_2-0\\\vdots\\p_n-0\end{bmatrix}=
\begin{bmatrix}p_1\\p_2\\\vdots\\p_n\end{bmatrix}
\end{align*}

This definition is illustrated in the following picture for the special case of $\mathbb{R}^3$

```{image} ../Figures/fig4_00.png
:width: 300px
:align: center
```

</div>


We can also determine the **position vector from $P$ to $Q$** (the vector from $P$ to $Q$) as follows
\begin{align*}
\overrightarrow{PQ}=\begin{bmatrix}q_1\\q_2\\\vdots\\q_n\end{bmatrix}-\begin{bmatrix}p_1\\p_2\\\vdots\\p_n\end{bmatrix}=
\begin{bmatrix}q_1-p_1\\q_2-p_2\\\vdots\\q_n-p_n\end{bmatrix}=\overrightarrow{0Q}-\overrightarrow{0P}.
\end{align*}
where $P = (p_1 ,\ldots,p_n )$ and $Q = (q_1 ,\ldots,q_n )$.

```{image} ../Figures/fig4_01.png
:width: 450px
:align: center
```

***
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***