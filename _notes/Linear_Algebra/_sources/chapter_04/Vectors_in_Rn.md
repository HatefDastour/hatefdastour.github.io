# Vectors in $\mathbb{R}^n$

-   A scalar quantity has only magnitude. Examples: time, temp,
    distance, speed,...

-   A vector quantity has both magnitude and direction. Examples:
    displacement, velocity, force,...
    
**Ordered n-tuple**: An ordered sequence $(a_1 , a_2 , \ldots, a_n )$ of real numbers is called an \textbf{ordered n-tuple}. The word “ordered” here reflects our insistence that two ordered n-tuples are equal if and only if corresponding entries are the same. In other words,

$$(a_1 , a_2 , \ldots, a_n ) = (b_1 , b_2 , \ldots, b_n )$$

if and only if

$$a_1 = b_1 , a_2 = b_2 , \ldots,\text{ and }a_n = b_n$$


The notation $\mathbb{R}^n$ refers to the collection of ordered lists of $n$
real numbers, that is
$$\mathbb{R}^n =\left\{ (x_1,\ldots,x_n ):~x_j \in \mathbb{R}~\text{for}~j = 1,\ldots ,n\right\}.$$
For example,

-   $n=1$: $\mathbb{R}=\mathbb{R}^1 =\left\{x_1:~x_1 \in \mathbb{R}\right\}.$
    $$1$, $\sqrt{2}$, $\frac{3}{2}$,...are points in $\mathbb{R}$.

-   $n=2$: $\mathbb{R}^2 =\left\{ (x_1,x_2 ):~x_1,x_2 \in \mathbb{R}\right\}$.
    $($1,2)$, $(\sqrt{2},2)$, $\left(\frac{3}{2},0\right)$,...are points in $\mathbb{R}^2.$

-   $n=3$: $\mathbb{R}^3 =\left\{ (x_1,x_2,x_3 ):~x_1,x_2,x_3 \in \mathbb{R}\right\}$.
    $(1,2,3)$, $(\sqrt{2},2,1)$, $\left(\frac{3}{2},0,\sqrt{5}\right)$,...are points in $\mathbb{R}^3$.

**Vectors in $\mathbb{R}^n$**: Let $\mathbb{R}^n =\left\{ (x_1,\ldots,x_n ):~x_j \in \mathbb{R}~\text{for}~j = 1,\ldots ,n\right\}$. Then $\vec{x}=\begin{bmatrix} x_1\\ \vdots \\ x_n \\  \end{bmatrix}$ is called a  \textbf{vector}. Vectors have both size (magnitude) and direction. The numbers $x_j$ are called the \textbf{components} of $\vec{x}$.

**The origin**: The point given by $0 = (0,\ldots ,0)$ is called the origin.

**The Position Vector**: Position vector is the vector which represents the position of a point in a space with respect to the origin 0. Let $P = (p_1 ,\ldots,p_n )$ be the coordinates of a point in $\mathbb{R}^n$ . Then the vector $\overrightarrow{0P}$  with its tail at $0 =(0,\ldots ,0)$ and its tip at $P$ is called the position vector of the point $P$. We write
\begin{align*}
\overrightarrow{0P}=\begin{bmatrix}p_1\\p_2\\\vdots\\p_n\end{bmatrix}-\begin{bmatrix}0\\0\\\vdots\\0\end{bmatrix}
=\begin{bmatrix}p_1-0\\p_2-0\\\vdots\\p_n-0\end{bmatrix}=
\begin{bmatrix}p_1\\p_2\\\vdots\\p_n\end{bmatrix}
\end{align*}

This definition is illustrated in the following picture for the special case of $\mathbb{R}^3$

```{image} ../Figures/fig4_00.png
:width: 450px
:align: center
```

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
<ol>
<li><p>Vectors can be written in either <strong>column vector</strong> form or <strong>row vector</strong> form <span class="math display">\[\begin{aligned}
\vec{u}&=\begin{bmatrix}    u_1\\ \vdots \\ u_n \\  \end{bmatrix},& {(\text{column vector})}\\
\vec{u}&=\begin{bmatrix}    u_1 & \dots & u_n \\  \end{bmatrix}.& {(\text{row vector})}\end{aligned}\]</span></p></li>
<li><p>Sometimes a <strong>column vector</strong> in <span class="math inline">\(\mathbb{R}^n\)</span> is written in forms of <span class="math inline">\(\begin{bmatrix}    u_1 & \dots & u_n \\  \end{bmatrix}^T\)</span>.</p></li>
</ol>
</div>

We can also determine the \textbf{position vector from $P$ to $Q$} (the vector from $P$ to $Q$) as follows
\begin{align*}
\overrightarrow{PQ}=\begin{bmatrix}q_1\\q_2\\\vdots\\q_n\end{bmatrix}-\begin{bmatrix}p_1\\p_2\\\vdots\\p_n\end{bmatrix}=
\begin{bmatrix}q_1-p_1\\q_2-p_2\\\vdots\\q_n-p_n\end{bmatrix}=\overrightarrow{0Q}-\overrightarrow{0P}.
\end{align*}
where $P = (p_1 ,\ldots,p_n )$ and $Q = (q_1 ,\ldots,q_n )$.

```{image} ../Figures/fig4_01.png
:width: 200px
:align: center
```

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
