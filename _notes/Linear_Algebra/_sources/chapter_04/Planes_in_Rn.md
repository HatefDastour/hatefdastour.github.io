# Planes in $\mathbb{R}^n$

## Normal Vector
If a nonzero vector $\vec{n}$ is perpendicular to every vector from a plane, then vector $\vec{n}$ is called a **normal** for the plane. We know that two nonzero vectors $\vec{v}$ and $\vec{n}$ are perpendicular when their dot product is zero. That is,
\begin{equation*}
\vec{v} \bullet \vec{n}=0 \quad \text{or}\quad \vec{n} \bullet \vec{v}=0.
\end{equation*}

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Normal Vector
</b></font>

A nonzero vector in $\vec{n} \in \mathbb{R}^n$) is called a \textbf{normal vector} to a plane if and only if
\begin{align*}
\vec{n}\bullet \vec{v} = 0
\end{align*}
for every vector $\vec{v}$ in the plane.
```{image} ../Figures/fig4_18.png
:width: 220px
:align: center
```
  
</div>

## Vector Equation of a Plane

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Vector Equation of a Plane
</b></font>

Consider a plane with the normal vector $\vec{n}$. Let point $P_0$ be on this plane. Then, any point $P$ on this plane can be expressed as follows,
\begin{equation*}
\vec{n}\bullet \left(\overrightarrow{0P}-\overrightarrow{0P_0}\right)=0.
\quad \text{or} \quad
\overrightarrow{P_0P} \bullet \vec{n}=0.
\end{equation*}
This is called the **vector equation** of a plane.

```{image} ../Figures/fig4_19.png
:width: 300px
:align: center
```  
</div>

In $\mathbb{R}^3$, the plane that contains point $P_0=(x_0,~y_0,~z_0)$
and has the normal vector $\vec{n} =(a,~b,~c)\neq 0$ is given by
\begin{equation*}
a(x-x_0 )+b(y-y_0 )+c(z-z_0 ) = 0.
\end{equation*}


<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
A point $P=(x,~y,~z)$ is on a plane if and only if $x$ , $y$ , and $z$ satisfy its vector equation.
</div>

<font color='Blue'><b>Example</b></font>:
Find an equation of the plane containing $(1,-1,0)$  and orthogonal to $\begin{bmatrix} \pi & 0 & 3 \end{bmatrix}^T$.

<font color='Green'><b>Solution</b></font>:
Here $P_0=(1,-1,0)$ and $\vec{n} =(\pi,0,3)$
\begin{align*}
\pi(x-1 )+0(y-(-1) )+3(z-0 ) = 0 \quad \Rightarrow \quad \pi x +3z=\pi.
\end{align*}
***

## Scalar Equation of a Plane

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Scalar Equation of a Plane
</b></font>

Assume that $\vec{n} = \begin{bmatrix}  a & b & c \end{bmatrix}^T$ is a normal vector of a plance and this plance also includes points $P_0 = (x_0,~y_0,~z_0)$. Then, for any given point $P = (x,~y,~z)$ on this plane, the **scalar equation** of the plane is given by
\begin{equation*}
ax+by+cz = d
\end{equation*}
where $a,~b,~c,~d \in \mathbb{R}$ and $d = ax_0 +by_0 +cz_0$.
</div>

<font color='Blue'><b>Example</b></font>:
Let $A = (0,0,1)$, $B = (2,0,-1)$ and $C = (0,1,0)$ be points in $\mathbb{R}^3$. Find an equation for the plane containing $A$, $B$, and $C$.

<font color='Green'><b>Solution</b></font>:
The scalar equation of the plane is given by $ax+by+cz = d$ where $a,~b,~c,~d$ are to be determined. To find $a,~b,~c,~d$, we use points $A$, $B$ and $C$. We have

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

{badge}`In RREF:,badge-primary`

\begin{equation*}
\left[\begin{array}{cccc|c} {1} & 0 & 0 & -1 & 0\\ 0 & {1} & 0 & -1 & 0\\ 0 & 0 & {1} & -1 & 0 \end{array}\right]
\end{equation*}


<center>
<table style="border-collapse:collapse;border-spacing:0" class="tg"><thead><tr><th style="border-color:inherit;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">Basic variables</th><th style="border-color:inherit;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">Free variable</th></tr></thead><tbody><tr><td style="border-color:inherit;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">a, b and c</td><td style="border-color:inherit;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;text-align:center;vertical-align:top;word-break:normal">d</td></tr></tbody></table>
</center>


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
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
