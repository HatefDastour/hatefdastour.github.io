# Worksheet 06

1. Compute the Wronskians of the given sets of functions.

* a). $\{e^x, e^x \sin x\}$,
* b). $\{ x^{1/2},  x^{-1/3}\}$.
    
<font color='Green'><b>Solution</b></font>:

* a). 
\begin{align*}
W(x)=\begin{vmatrix}
e^x & e^x \sin x \\
e^x & e^x\,\cos\left(x\right)+e^x\,\sin\left(x\right)
\end{vmatrix}=e^{2\,x}\,\cos\left(x\right).
\end{align*}
* b). 

\begin{align*}
W(x)=\begin{vmatrix}
\sqrt{x} & \frac{1}{x^{1/3}}\\ \frac{1}{2\,\sqrt{x}} & -\frac{1}{3\,x^{4/3}}
\end{vmatrix}=-\frac{5}{6\,x^{5/6}}.
\end{align*}


***

`````{admonition} Abel's Formula
:class: important

Consider the second-order linear homogeneous differential equation:

\begin{equation}\label{eq:5.1.27}
y''+p(x)y'+q(x)y=0,
\end{equation}

where $p(x)$ and $q(x)$ are continuous functions defined on the interval $(a,b)$. Let $y_1(x)$ and $y_2(x)$ be two solutions of this equation on $(a,b)$. We define the Wronskian as:

\begin{equation}\label{eq:5.1.28}
W=y_1y_2'-y_1'y_2.
\end{equation}

For any point $x_0$ in the interval $(a,b)$, Abel's formula states:

\begin{equation} \label{eq:5.1.29}
W(x)=W(x_0) e^{-\int_{x_0}^x p(t)\, dt}, \quad a<x<b.
\end{equation}

Consequently, either the Wronskian $W$ has no zeros in the interval $(a,b)$, or it is identically equal to zero on $(a,b)$.

This result, known as Abel's formula, provides a useful relationship between the Wronskian and the integrating factor involving the function $p(x)$ in the given differential equation. For further information on Abel and his contributions, you can refer to [Abel's
biography](http://www-history.mcs.st-and.ac.uk/Mathematicians/Abel.html).
`````


2. Find the Wronskian of a given set $\{y_1,y_2\}$ of solutions of
\begin{align*}
x^2y''+xy'+(x^2-\nu^2)y=0 ,
\end{align*}
given that $W(1)=1$.
    
<font color='Green'><b>Solution</b></font>:

Note that $p(x)=\dfrac{1}{x}$. Thus,
\begin{align*}
\int^x_{x_0}p(t)\,dt= {\int_1^x  p(t)\,dt}={\int_1^x\frac{1}{t}dt}=\ln x,\end{align*}
and Abel's
formula yields
\begin{align*}W(x)=W(1)e^{-\ln x}=\frac{1}{x}.\end{align*}


***

`````{admonition} Fundamental Set of Solutions
:class: important
    
Suppose $p$ and $q$ are continuous functions, and $y_1$ is a solution of the second-order linear homogeneous differential equation:

$$
y''+p(x)y'+q(x)y=0 \quad \text{(A)}
$$

with no zeros on the interval $(a,b)$. Let $P(x)$ be any antiderivative of $p(x)$ on $(a,b)$.

* (a) If $K$ is a nonzero constant and $y_2$ satisfies the following equation on $(a,b)$:

$$
y_1y_2'-y_1'y_2=Ke^{-P(x)} \quad \text{(B)}
$$

then $y_2$ also satisfies equation (A) on $(a,b)$, and the pair $\{y_1,y_2\}$ forms a fundamental set of solutions for equation (A) on $(a,b)$.

* (b) If $y_2=uy_1$, where $u'=K\frac{e^{-P(x)}}{y_1^2(x)}$, then $\{y_1,y_2\}$ forms a fundamental set of solutions for equation (A) on $(a,b)$.

In both cases, the given conditions and relationships ensure that $y_1$ and $y_2$ satisfy equation (A) on the interval $(a,b)$ and together form a fundamental set of solutions.
`````



3. For the given ODE, find a second solution $y_2$ that isn't a constant multiple of the solution $y_1$. Choose $K$ conveniently to simplify
$y_2$.

* a). $y''-2ay'+a^2y=0,\quad (a=\text{ constant, and })  \quad  y_1=e^{ax}$
* b).  $x^2y''-xy'+y=0,  \quad y_1=x$
    
<font color='Green'><b>Solution</b></font>:

* a). We can see that $p(x)=-2a$. Then, $P(x)= \int p(x)\,dx = -2ax$. Moreover, letting
$y_2=uy_1=ue^{ax}$, leads to
\begin{align*}u'=K\frac{e^{-P(x)}}{y_1^2(x)}=K\frac{e^{2ax}}{ e^{2ax}}=K.\end{align*}
Therefore, $u=\int K~dx=Kx$.

As $K$ is an arbitrary nonzero constant, choosing $K=1$ gives 
\begin{align*}
y_2=xe^{ax}.
\end{align*}

* b). Here, $p(x)=-{1\over x}$, then $P(x)=-\ln x$. Moreover, let
$y_2=uy_1=ux$. It follows that
\begin{align*}u'=K \frac{e^{-P(x)}}{ y_1^2(x)}=K\frac{x}{ x^2}={K}\frac{1}{ x}.\end{align*}
Thus, $u=K\ln x$. Letting $K=1$, then $y_2=x\ln x$.


***


`````{admonition} General solution for the second-order homogeneous linear ODE
:class: important
    
Consider the second-order homogeneous linear ordinary differential equation with constant coefficients:

\begin{equation}\label{eq2.1.01}
a_{2} y''(x)+a_{1} y'(x)+a_{0} y(x)=0,
\end{equation}

where $a_0$, $a_1$, and $a_2$ are arbitrary constants.

To find the characteristic equation corresponding to the ODE \eqref{eq2.1.01}, we can set up the following equation:

\begin{equation}\label{HOL-eq.02}
a_{2} r^2+a_{1} r+a_{0}=0.
\end{equation}

Let $r_1$ and $r_2$ be the two roots of this characteristic equation. Depending on the nature of the roots, we can consider the following cases to find a general solution for the corresponding ODE:

* (a) If the characteristic equation has distinct real roots, $r_1$ and $r_2$, the general solution is given by:

\begin{equation}
y(x) = c_1 e^{r_1 x} +c_2 e^{r_2 x}.
\end{equation}

* (b) If the characteristic equation has a pair of complex roots, $\alpha \pm \beta i$, the general solution is given by:

\begin{equation}
y(x) = e^{\alpha x}\left(c_1 \cos(\beta x)+c_2\sin(\beta x)\right).
\end{equation}

* (c) If $r_1$ is a repeated root of the characteristic equation (i.e., $r_1=r_2$), the general solution is given by:

\begin{equation}
y(x) = c_1 e^{r_1 x} +c_2 x e^{r_1 x}.
\end{equation}

`````



4. Find the general solution.
* a). $y''-4y'+5y=0$,
* b). $y''-4y'+4y=0$,
* c). $y''+6y'+10y=0$,
* d). $6y''-y'-y=0$, with  $y(0)=10$, and $y'(0)=0$.
    
<font color='Green'><b>Solution</b></font>:

* a).
$p(r)=r^2-4r+5=(r-2)^2+1$.

Since $r_1,r_2=2\pm i$, then
\begin{align*}y=e^{2x}(c_1 \cos x+c_2 \sin x).\end{align*}

* b).
$p(r)=r^2-4r+4=(r-2)^2$.

Since $r_1,r_2=2$, then
\begin{align*}y=e^{2x}(c_1+c_2x).\end{align*}

* c).
$p(r)=r^2+6r+10=(r+3)^2+1$.

Since $r_1,r_2=-3\pm i$, then
\begin{align*}y=e^{-3x}(c_1 \cos x+c_2 \sin x).\end{align*}

* d). $p(r)=6r^2-r-1=(2r-1)(3r+1)=6(r-1/2) (r+1/3)$. Thus,
\begin{align*}
y=c_1e^{-x/3}+c_2e^{x/2}
\end{align*}
Moreover,
$y'=-\dfrac{c_1}{3}e^{-x/3}+\dfrac{c_2}{2}e^{x/2}$. Now,
\begin{align*}\begin{cases}
  y(0)=10\Rightarrow c_1+c_2=10\\
  y'(0)=0\Rightarrow -{c_1\over3}+{c_2\over2}=0.
\end{cases}
\end{align*}
Hence, $c_1=6, c_2=4$, and $y=4e^{x/2}+6e^{-x/3}$.


***
**Refrences**

1. Trench, William F. "Elementary differential equations with boundary value problems." (2018).
***