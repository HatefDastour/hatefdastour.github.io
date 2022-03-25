# 4.4 Length of a Vector

Let $P$ and $Q$ be two points in $\mathbb{R}^n$,

-   $n=1$: distance= $d(P,Q)=|P-Q|$

-   $n=2$: distance= $d(P,Q)=\sqrt{(p_1-q_1)^2+(p_2-q_2)^2}$

```{image} ../Figures/fig4_07.png
:width: 300px
:align: center
```

-   $n=3$: distance= $d(P,Q)=\sqrt{(p_1-q_1)^2+(p_2-q_2)^2+(p_3-q_3)^2}$

```{image} ../Figures/fig4_08.png
:width: 400px
:align: center
```

**Distance Between Points**: Let $P = (p_1,\ldots,p_n)$ and $Q=(q_1,\ldots,q_n)$ be two points in $\mathbb{R}^n$. Then the distance between these points is defined as
\begin{align*}
%\text{distance between $P$ and $Q$}=
d(P,Q)=%\left(\sum_{k=1}^{n}|p_k-q_k|^2\right)^{\frac{1}{2}}
\sqrt{(p_1-q_1)^2+(p_2-q_2)^2+(p_3-q_3)^2+\ldots+(p_n-q_n)^2}
\end{align*}
This is called the \textbf{distance formula}. We may also write $|P-Q|$ as the distance between $P$ and $Q$.

<font color='Blue'><b>Example</b></font>:
Find the distance between the points $P$ and $Q$ in $\mathbb{R}^6$ , where $P$ and $Q$ are given by $P =\left(1, 2 , 1 , 3 , 3 , 4 \right)$ and $Q=\left( 0 , 1 , 0 , 1 , 0 , 1 \right)$.
***
<font color='Green'><b>Solution</b></font>:
\begin{align*}
\text{distance}=\sqrt{(0-1)^2+(1-2)^2+(0-1)^2+(1-3)^2+(0-3)^2+(1-4)^2}=\sqrt{25}=5
\end{align*}
***

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem:
</b></font>
    
<p>Let <span class="math inline">\(P\)</span> and <span class="math inline">\(Q\)</span> be points in <span class="math inline">\(R^n\)</span>, and let the distance between them. Then, the following properties hold.</p>
<ul>
<li><p><span class="math inline">\(d(P,Q) = d(Q,P)\)</span></p></li>
<li><p><span class="math inline">\(d(P,Q) \geq 0\)</span>,.</p></li>
<li><p>If <span class="math inline">\(d(P,Q)=0\)</span>, then <span class="math inline">\(P = Q\)</span>.</p></li>
</ul>
    
</div>

**Length of $\overrightarrow{PQ}$**: Let $P = (p_1,\ldots,p_n)$ and $Q=(q_1,\ldots,q_n)$ be two points in $\mathbb{R}^n$. The distance between $\vec{P}$ and $\vec{Q}$ is the length of $\overrightarrow{PQ}$,
\begin{align*}
\|\overrightarrow{PQ}\|=\sqrt{(p_1-q_1)^2+(p_2-q_2)^2+(p_3-q_3)^2+\ldots+(p_n-q_n)^2}
\end{align*}

**Length of a Vector**: Let $\vec{u} = \left[u_1,\ldots,u_n\right]^T$ be a vector in $\mathbb{R}^n$. Then, the length of $\vec{u}$, written $\|\vec{u}\|$ is given by
\begin{align*}
\|\vec{u}\|=\sqrt{u_1^2+\ldots+u_n^2}
\end{align*}

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
<p>Let <span class="math inline">\(\vec{u}=\begin{bmatrix}u_1 & u_2 & \dots & u_n\end{bmatrix}^T\)</span> be a vector in <span class="math inline">\(\mathbb{R}^n\)</span>. For a scalar <span class="math inline">\(k\in \mathbb{R}\)</span>, <span class="math display">\[\begin{aligned}
\|ku\|=|k|\| u \|=|k|\sqrt{u_1^2+\ldots+u_n^2}\end{aligned}\]</span> where <span class="math inline">\(|k|\)</span> is the absolute value of <span class="math inline">\(k\)</span>.</p>
    
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

**Unit Vector and Normalized Vector**: Let $\vec{u}$ be a vector in $\mathbb{R}^n$. Then, we call $\vec{u}$ a unit vector if it has length 1, that is if $\|\vec{u}\|=1$.

If $\|\vec{v}\|\neq0$, we can normalize a vector $\vec{v} \in \mathbb{R}^n$ by

$$\vec{u}=\frac{1}{\|\vec{v}\|}\vec{v},$$

where the vector $\vec{u}$ has the same direction as $\vec{v}$ but length equal to 1.

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
First off,
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
:width: 300px
:align: center
```

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
