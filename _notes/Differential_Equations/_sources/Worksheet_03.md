# Worksheet 03

1. Find the general solution.
* *a)* $(\sec^2y)y'- 3\tan y=-1$,
* *b)* $e^{y^2}\left(2yy'+ \frac{2}{x}\right) =\frac{1}{x^2}$.
    
<font color='Green'><b>Solution</b></font>:

* *a)* Let $z = \tan(y)$, then $z' = \sec^2(y)y'$. Thus,

$$z'- 3z=-1$$

Now, the above equation is a first order linear ODE with $p(x) = -3$ and $q(x) = -1$. Therefore,

\begin{align*}
& \mu(x) = e^{\int -3 dx}= e^{-3x},\\
\Rightarrow \quad & \frac{d}{dx}\left(e^{ax} z \right) = \left(e^{ax}\right)\left(0\right),\\
\Rightarrow \quad & e^{-3x}z = \int -e^{-3x} dx = \frac{1}{3}e^{-3x}+c, \quad c \in \mathbb{R},\\
\Rightarrow \quad & z = \frac{1}{3}+ce^{3x}, \quad c \in \mathbb{R}.
\end{align*}

Now, since $z = \tan(y)$,

$$y = \tan^{-1}\left(\frac{1}{3}+ce^{3x}\right), \quad c \in \mathbb{R}.$$

* *b)* Let $z = \exp\left(y^2\right)$, then $z' = 2yy'\exp\left(y^2\right)$. Thus,

$$z' +\frac{2}{x}z=\frac{1}{x^2}$$

Now, the above equation is a first order linear ODE with $p(x) = \frac{2}{x}$ and $q(x) = \frac{1}{x^2}$. Therefore,

\begin{align*}
& \mu(x) = e^{\int 2/x dx}= \exp\left(2\ln|x|\right) = |x|^2 = x^2,\\
\Rightarrow \quad & \frac{d}{dx}\left( x^2 z \right) = \left( x^2 \right)\left(\frac{1}{x^2}\right) = 1,\\
\Rightarrow \quad & x^2 z = x + c, \quad c \in \mathbb{R},\\
\Rightarrow \quad & z = \frac{1}{x}+\frac{c}{x^2}, \quad c \in \mathbb{R}.
\end{align*}

Now, since $z = \exp\left(y^2\right)$,

\begin{align*}\exp\left(y^2\right) = \frac{1}{x}+\frac{c}{x^2}, \quad c \in \mathbb{R}.\end{align*}
and
\begin{align*}y = \pm \sqrt{\ln\left( \frac{1}{x}+\frac{c}{x^2} \right)}, \quad c \in \mathbb{R}.\end{align*}

***

2. Find all solutions.
* *a)* $y'=\dfrac{3x^2+2x+1}{y-2}$,
* *b)* $(\sin(x))(\sin(y))+(\cos(y))y'=0$.

<font color='Green'><b>Solution</b></font>:

* *a)* As can be seen, the ODE is separable. Thus,

\begin{align*}
& y' = \dfrac{3x^2 + 2x +1}{y-2},\\
\Rightarrow \quad & \frac{dy}{dx}= \dfrac{3x^2 + 2x +1}{y-2},\\
\Rightarrow \quad & (y-2)dy= \left(3x^2 + 2x +1\right) dx,\\
\Rightarrow \quad & \int(y-2)dy= \int\left(3x^2 + 2x +1\right) dx,\\
\Rightarrow \quad & \frac{1}{2}y^2-2y = x^3 + x^2 +x +c, \quad c \in \mathbb{R}.
\end{align*}

* *b)* It can be seen that the ODE is separable. Therefore,

\begin{align*}
& -(\sin(x))(\sin(y)) = (\cos(y))\frac{dy}{dx},\\
\Rightarrow \quad & -\sin(x)dx = \frac{\cos(y)}{\sin(y)}dy,\\
\Rightarrow \quad & \int-\sin(x)dx = \int\frac{\cos(y)}{\sin(y)}dy,\\
\Rightarrow \quad & \cos(x) + c = \ln|\sin(y)|, \quad c \in \mathbb{R}.
\end{align*}

***
**Refrences**

1. Trench, William F. "Elementary differential equations with boundary value problems." (2018).
***