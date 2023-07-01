# Worksheet 02

1. Find the general solution.
* *a)* $y'+ay=0$ ($a$=constant),
* *b)* $xy'+3y=0$,
* *c)* $y'+2xy=xe^{-x^2}$,
* *d)* $xy'+(1+2x^2)y=x^3e^{-x^2}$.
    
<font color='Green'><b>Solution</b></font>:

`````{admonition} For a first order linear ODE
:class: important
    
Consider the first order linear ordinary differential equation (ODE):

\begin{align*}
y' + p(x) y = q(x).
\end{align*}

Let's introduce an integrating factor $\mu(x) = \exp\left(p(x)dx\right)$ for this ODE.

Using this integrating factor, we can rewrite the equation as follows:

\begin{align*}
\mu(x)y' + \mu(x)p(x) y = \mu(x)q(x).
\end{align*}

Now, let's simplify this expression further. Note that $\mu(x) = \exp\left(p(x)dx\right)$, so we have:

\begin{align*}
\mu(x)y' + \mu(x)p(x) y &= \exp\left(p(x)dx\right)y' + \exp\left(p(x)dx\right)p(x) y \\
&= \frac{d}{dx}\left(\exp\left(p(x)dx\right)y\right).
\end{align*}

Thus, we can rewrite the equation as:

\begin{align*}
\frac{d}{dx}\left(\mu(x)y\right) = \mu(x)q(x).
\end{align*}

This is a convenient form of the equation that allows us to solve it more easily.

`````

* *a)* Note that $p(x) = a$ and $q(x) = 0$. Therefore,

\begin{align*}
& \mu(x) = e^{\int a dx}= e^{ax},\\
\Rightarrow \quad & \frac{d}{dx}\left(e^{ax} y \right) = \left(e^{ax}\right)\left(0\right),\\
\Rightarrow \quad & e^{ax}y = \int 0 dx = c, \quad c \in \mathbb{R},\\
\Rightarrow \quad & y = ce^{-ax}, \quad c \in \mathbb{R}.
\end{align*}

* *b)* We have $y'+\dfrac{3}{x}y=0$

Now $p(x) = \dfrac{3}{x}$ and $q(x) = 0$. Therefore,

\begin{align*}
\mu(x) = e^{\int \frac{3}{x} dx}= e^{3 \ln|x|} = |x|^3
\end{align*}

We can use either $\mu(x) = x^3$ or $\mu(x) = -x^3$. Using $\mu(x) = x^3$, we have
\begin{align*}
& \frac{d}{dx} \left( x^3 y \right) = \left(x^3 \right)\left(0\right),\\
\Rightarrow \quad & x^3 y = \int 0 dx = c, \quad c \in \mathbb{R},\\
\Rightarrow \quad & y = \frac{c}{x^3}, \quad c \in \mathbb{R}.
\end{align*}

* *c)* $p(x) = 2x$ and $q(x) = x e^{-x^2}$. Therefore,

\begin{align*}
& \mu(x) = e^{\int 2x dx}= e^{x^2},\\
\Rightarrow \quad & \frac{d}{dx}\left(e^{x^2} y \right) = x \left(e^{x^2}\right)\left(e^{x^{-2}}\right) =x,\\
\Rightarrow \quad & e^{x^2} y  = \int x dx = \frac{1}{2} x^2 + c, \quad c \in \mathbb{R},\\
\Rightarrow \quad & y  = \int x dx = \frac{1}{2} x^2e^{-x^2}  + ce^{-x^2} , \quad c \in \mathbb{R},\\
\end{align*}

* *d)* We have $y'+ \left(\dfrac{1}{x}+2x \right)y=x^2e^{-x^2}$, and then $p(x) = \dfrac{1}{x}+2x$ and $q(x) = x^2e^{-x^2}$. Therefore,

\begin{align*}
\mu(x) = \exp \left(\int \left(\frac{1}{x}+2x  \right)dx\right) = \exp \left( \ln |x| + x^2\right)=
\exp \left( \ln |x|\right) \exp \left( x^2\right)
\end{align*}

We can use either $\mu(x) = x e^{x^2}$ or $\mu(x) = -x e^{x^2}$. Using $\mu(x) = x e^{x^2}$, we have
\begin{align*}
& \frac{d}{dx} \left( x e^{x^2} y \right) = \left(x e^{x^2} \right)\left(x^2e^{-x^2}\right),\\
\Rightarrow \quad & x e^{x^2} y = \dfrac{1}{4}x^4 + c, \quad c \in \mathbb{R},\\
\Rightarrow \quad & y = e^{-x^2}\left( \dfrac{1}{4}x^3 + \dfrac{c}{x}\right), \quad c \in \mathbb{R}.
\end{align*}

***

2. Solve the initial value problem.
* *a)* $xy'+(1+ x\cot (x))y=0,\quad y\left(\dfrac{\pi}{4}\right)=2$,
* *b)* $y'+\dfrac{3}{x}y=\dfrac{\sin x}{x^2},\quad y\left(\dfrac{\pi}{2}\right)=1$.
    
<font color='Green'><b>Solution</b></font>:

* *a)* $y'+\left(\dfrac{1}{x}+ \cot x \right)y=0,\quad y\left(\dfrac{\pi}{2}\right)=2$,

$p(x) = a$ and $q(x) = 0$. Therefore,

\begin{align*}
\mu(x) & =\exp\left(\int\left(\dfrac{1}{x}+ \cot (x) \right) dx \right)= 
\exp\left(\ln|x| + \ln|\sin(x)| \right)
\\
&=\exp\left(\ln|x|\right) \exp\left( \ln|\sin(x)| \right) = |x||\sin(x)| 
\end{align*}

We can use either $\mu(x) = x\sin(x)$ or $\mu(x) = -x\sin(x)$. Using $\mu(x) = x\sin(x)$, we have

\begin{align*}
& \frac{d}{dx} \left( x\sin(x) y\right) = \left(x\sin(x) \right)\left(0\right),\\
\Rightarrow \quad & x\sin(x) y= \int 0 dx = c, \quad c \in \mathbb{R},\\
\Rightarrow \quad &  y=  \dfrac{c}{x\sin(x)}, \quad c \in \mathbb{R}.
\end{align*}

Moreover, since $y\left(\dfrac{\pi}{4}\right)=2$,
\begin{align*}
& 2 = \dfrac{c}{\frac{\pi}{4} \sin\left(\frac{\pi}{4}\right)},\\
\Rightarrow \quad &  c = 2\left(\frac{\pi}{4} \sin\left(\frac{\pi}{4}\right)\right)=\frac{\pi}{4}\sqrt{2}.
\end{align*}


* *b)* $y'+\dfrac{3}{x}y= \dfrac{\sin(x)}{x^2},\quad y\left(\dfrac{\pi}{2}\right)=1$,

$p(x) = \frac{3}{x}$ and $q(x) = \frac{\sin(x)}{x^2}$. Therefore,

\begin{align*}
\mu(x) & =\exp\left(\int\dfrac{3}{x} dx \right) = |x|^3
\end{align*}

We can use either $\mu(x) = x^3$ or $\mu(x) = -x^3$. Using $\mu(x) = x^3$, we have

\begin{align*}
& \frac{d}{dx} \left( x^3 y\right) = \left(x^3 \right)\left(\frac{\sin(x)}{x^2}\right),\\
\Rightarrow \quad &  x^3 y= \int x\sin(x)dx,\\
\Rightarrow \quad &  x^3 y= -x\cos(x) + \sin(x) + c,\quad c \in \mathbb{R},\\
\Rightarrow \quad &  y= - \dfrac{\cos(x)}{x^2} + \dfrac{\sin(x)}{x^3} + \dfrac{c}{x^3},\quad c \in \mathbb{R},\\
\end{align*}

Moreover, since $y\left(\dfrac{\pi}{2}\right)=1$,
\begin{align*}
c = \dfrac{\pi^3 - 8}{8}.
\end{align*}

***
**Refrences**

1. Trench, William F. "Elementary differential equations with boundary value problems." (2018).
***
