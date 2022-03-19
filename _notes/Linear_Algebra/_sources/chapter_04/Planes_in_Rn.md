# Planes in $\mathbb{R}^n$

A nonzero vector $n$ is called a normal for a plane if it is orthogonal to every vector in the plane.

**Normal Vector**:
Let $\vec{n}$ be a nonzero vector in $\mathbb{R}^n$. Then $\vec{n}$ is called a \textbf{normal vector} to a plane if and only if
$$
\vec{n}\bullet \vec{v} = 0
$$
for every vector $\vec{v}$ in the plane.

```{image} ../Figures/fig4_18.png
:width: 220px
:align: center
```

**Vector Equation of a Plane**: Let $\vec{n}$ be the normal vector for a plane which contains a point $P_0$. If $P$ is an arbitrary point on this plane, then the \textbf{vector equation} of the plane is given by
\begin{equation*}
\vec{n}\bullet \left(\overrightarrow{0P}-\overrightarrow{0P_0}\right)=0.
\quad \text{or} \quad
\overrightarrow{P_0P} \bullet \vec{n}=0.
\end{equation*}

```{image} ../Figures/fig4_19.png
:width: 300px
:align: center
```

The plane through $P_0=(x_0 , y_0 , z_0 )$ with normal\linebreak $\vec{n} =(a , b , c )\neq 0$ as a normal vector is given by
\begin{equation*}
a(x-x_0 )+b(y-y_0 )+c(z-z_0 ) = 0.
\end{equation*}
In other words, a point $P=(x, y, z)$ is on this plane if and only if $x$ , $y$ , and $z$ satisfy this equation.

<font color='Blue'><b>Example</b></font>:
Find an equation of the plane containing $(1,-1,0)$  and orthogonal to $\begin{bmatrix} \pi & 0 & 3 \end{bmatrix}^T$.

<font color='Green'><b>Solution</b></font>:
Here $P_0=(1,-1,0)$ and $\vec{n} =(\pi,0,3)$
\begin{align*}
\pi(x-1 )+0(y-(-1) )+3(z-0 ) = 0 \quad \Rightarrow \quad \pi x +3z=\pi.
\end{align*}
***

**Scalar Equation of a Plane**: Let $\vec{n} = \begin{bmatrix}  a & b & c \end{bmatrix}^T$ be the normal vector for a plane which contains the point $P_0 = (x_0 ,y_0 ,z_0 )$. Then if $P = (x,y,z)$ is an arbitrary point on the plane, the scalar equation of the plane is given by $ax+by+cz = d$
where $a,b,c,d \in \mathbb{R}$ and $d = ax_0 +by_0 +cz_0$.

<font color='Blue'><b>Example</b></font>:
Let $A = (0,0,1)$, $B = (2,0,-1)$ and $C = (0,1,0)$ be points in $\mathbb{R}^3$. Find an equation for the plane containing $A$, $B$, and $C$.

<font color='Green'><b>Solution</b></font>:
The scalar equation of the plane is given by $ax+by+cz = d$ where $a,b,c,d$ are to be determined. To find $a,b,c,d$, we use points $A$, $B$ and $C$. We have

\begin{align*}
\begin{cases}
a(0)+b(0)+c(1) = d\\
a(2)+b(0)+c(-1) = d\\
a(0)+b(1)+c(0) = d
\end{cases}
\quad \Rightarrow \quad
\begin{cases}
c=d\\ 2\,a-c=d \\ b=d
\end{cases}
\quad \Rightarrow \quad
\begin{cases}
c-d=0\\ 2\,a-c-d=0 \\ b-d=0
\end{cases}
\end{align*}
The augmented matrix of this system is given by
\begin{equation*}
\left[\begin{array}{cccc|c} 0 & 0 & 1 & -1 & 0\\ 2 & 0 & -1 & -1 & 0\\ 0 & 1 & 0 & -1 & 0 \end{array}\right]
\end{equation*}

In RREF:
\begin{equation*}
\left[\begin{array}{cccc|c} {1} & 0 & 0 & -1 & 0\\ 0 & {1} & 0 & -1 & 0\\ 0 & 0 & {1} & -1 & 0 \end{array}\right]
\end{equation*}


<table style="border-collapse:collapse;border-spacing:0" class="tg"><thead><tr><th style="border-color:inherit;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">Basic variables</th><th style="border-color:inherit;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">Free variable</th></tr></thead><tbody><tr><td style="border-color:inherit;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">a, b and c</td><td style="border-color:inherit;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">d</td></tr></tbody></table>


Therefore,
\begin{equation*}
\begin{bmatrix} a\\ b\\ c\\d \end{bmatrix}=t\begin{bmatrix} 1\\ 1\\ 1\\1 \end{bmatrix},\quad t\in \mathbb{R}
\end{equation*}
Letting $t=1$,
\begin{equation*}
\begin{bmatrix} a & b & c & d \end{bmatrix}^{T}=\begin{bmatrix} 1 & 1 & 1 & 1 \end{bmatrix}^{T}.
\end{equation*}
Therefore,
\begin{equation*}
x+y+z=1.
\end{equation*}

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
