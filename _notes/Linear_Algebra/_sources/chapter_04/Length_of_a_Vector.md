# Length of a Vector

Let $P$ and $Q$ be two points in $\mathbb{R}^n$,

-   $n=1$: For two points $P$ and $Q$, the distance= $d(P,Q)=|P-Q|$

-   $n=2$: For two points $P=(p_1,~p_2)$ and $Q=(q_1,~q_2)$, distance= $d(P,Q)=\sqrt{(p_1-q_1)^2+(p_2-q_2)^2}$

```{image} ../Figures/fig4_07.png
:width: 300px
:align: center
```

-   $n=3$: For two points $P=(p_1,~p_2,~p_3)$ and $Q=(q_1,~q_2,~q_3)$, distance= $d(P,Q)=\sqrt{(p_1-q_1)^2+(p_2-q_2)^2+(p_3-q_3)^2}$

```{image} ../Figures/fig4_08.png
:width: 400px
:align: center
```

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Distance Between Points
</b></font>

For any two points $P = (p_1,\ldots,p_n)$ and $Q=(q_1,\ldots,q_n)$ in $\mathbb{R}^n$, the distance between these points is defined as follows
\begin{align*}
%\text{distance between $P$ and $Q$}=
d(P,Q)=%\left(\sum_{k=1}^{n}|p_k-q_k|^2\right)^{\frac{1}{2}}
\sqrt{(p_1-q_1)^2+(p_2-q_2)^2+(p_3-q_3)^2+\ldots+(p_n-q_n)^2}
\end{align*}
This is known as the **distance formula**, and it can be also written as $|P-Q|$ which also represents the distance between $P$ and $Q$.
</div>

<font color='Blue'><b>Example</b></font>:
Find the distance between the points $P$ and $Q$ in $\mathbb{R}^6$ , where $P$ and $Q$ are given by $P =\left(1, 2 , 1 , 3 , 3 , 4 \right)$ and $Q=\left( 0 , 1 , 0 , 1 , 0 , 1 \right)$.

<font color='Green'><b>Solution</b></font>:
\begin{align*}
\text{distance}=\sqrt{(0-1)^2+(1-2)^2+(0-1)^2+(1-3)^2+(0-3)^2+(1-4)^2}=\sqrt{25}=5
\end{align*}
***

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem:
</b></font>
    
For two points $P$ and $Q$ from $\mathbb{R}^n$,

* $d(P,Q) = d(Q,P)$,
* $d(P,Q) \geq 0$,
* If $d(P,Q)=0$, then $P = Q$,

where $d(P,Q)$ denote the distance between these two points
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Length of a Vector
</b></font>

The length of $\vec{u} = \left[u_1,\ldots,u_n\right]^T$ is given by
\begin{align*}
\|\vec{u}\|=\sqrt{u_1^2+\ldots+u_n^2}
\end{align*}
where $\|\vec{u}\|$ shows the length of $\vec{u}$.
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Length of <span class="math inline">\(\overrightarrow{PQ}\)</span>
</b></font>

For two points $P = (p_1,\ldots,p_n)$ and $Q=(q_1,\ldots,q_n)$ in $\mathbb{R}^n$, the length of $\overrightarrow{PQ}$ can be regarded as the distance between $\vec{P}$ and $\vec{Q}$. Thus,
\begin{align*}
\|\overrightarrow{PQ}\|=\sqrt{(p_1-q_1)^2+(p_2-q_2)^2+(p_3-q_3)^2+\ldots+(p_n-q_n)^2}
\end{align*}
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
Assume that $\vec{u}=\begin{bmatrix}u_1 & u_2 & \dots & u_n\end{bmatrix}^T$ is a vector in $\mathbb{R}^n$, and $k\in \mathbb{R}$ is a scalar. Then,
\begin{align*}
\|ku\|=|k|\| u \|=|k|\sqrt{u_1^2+\ldots+u_n^2}
\end{align*}
where $|k|$ shows the absolute value of $k$.
    
</div>

<font color='Blue'><b>Example</b></font>:
Let $\vec{u}=\begin{bmatrix}1 & 2 & 2\end{bmatrix}^T$. Then the length of $4\vec{u}=\begin{bmatrix}4 & 8 & 8\end{bmatrix}^T$ can be evaluated using
\begin{align*}
\|4u\|&=\sqrt{16+64+64}=\sqrt{144}=12
\\
&\text{or}
\\
\|4u\|&=|4|\sqrt{1+4+4}=4\sqrt{9}=(4)(3)=12.
\end{align*}

**Unit Vector**:A vector $\vec{u} \in \mathbb{R}^n$ is called if it's length is equal to 1 (i.e. $\|\vec{u}\|=1$).

If $\|\vec{v}\|\neq0$, we can normalize a vector $\vec{v} \in \mathbb{R}^n$ by

\begin{align*}\vec{u}=\frac{1}{\|\vec{v}\|}\vec{v}.\end{align*}

Observe that the vector $\vec{u}$ is aligned with $\vec{v}$ (has the same direction), but its length is 1.

```{image} ../Figures/fig4_09a.jpg
:height: 100px
:align: center
```

<font color='Blue'><b>Example</b></font>:
Let $\vec{v}$ be given by $\vec{v} =\begin{bmatrix} 1 & 2 & 2\end{bmatrix}^{T}$. Find the unit vector $\vec{u}$ which has the same direction as $\vec{v}$.

<font color='Green'><b>Solution</b></font>:
We have
\begin{align*}
\|\vec{v}\|=\sqrt{1+4+4}=3\neq0.
\end{align*}
Hence,
\begin{align*}
\vec{u}=\frac{1}{\|\vec{v}\|}\vec{v}=\frac{1}{3}\begin{bmatrix} 1 \\ 2 \\ 2\end{bmatrix}=\begin{bmatrix} 1/3 \\ 2/3 \\ 2/3\end{bmatrix}.
\end{align*}
We always can verify that $\|\vec{u}\|=1$.
***

<font color='Blue'><b>Example</b></font>:
Find the point $T$ which is $\dfrac{2}{3}$ of the way from $P=(3,-1,2)$ to $Q=(9,-7,-10)$.

<font color='Green'><b>Solution</b></font>:
First, let's calculate the lenght of $\overrightarrow{PQ}$,
```{image} ../Figures/fig4_09.png
:width: 200px
:align: center
```
\begin{equation*}
\overrightarrow{PQ}=\begin{bmatrix} 9\\-7\\-10\end{bmatrix}-\begin{bmatrix} 3\\-1\\2\end{bmatrix}=\begin{bmatrix} 6\\-6\\-12\end{bmatrix}.
\end{equation*}
Moreover, $T$ is $2/3$ of way from $P$ to $Q$. Therefore,
\begin{equation*}
\overrightarrow{PT}=\frac{2}{3}\overrightarrow{PQ}=\frac{2}{3}\begin{bmatrix} 6\\-6\\-12\end{bmatrix}=\begin{bmatrix} 4\\-4\\-8\end{bmatrix}
\end{equation*}
However, we need to find $T$. We know that
\begin{equation*}
\overrightarrow{0T}=\overrightarrow{0P}+\overrightarrow{PT}=
\begin{bmatrix} 3\\-1\\2\end{bmatrix}+\begin{bmatrix} 4\\-4\\-8\end{bmatrix}=\begin{bmatrix} 7\\-5\\-6\end{bmatrix}
\end{equation*}

```{image} ../Figures/fig4_10.png
:width: 320px
:align: center
```

***
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
