# Worksheet 04

1. Solve the given Bernoulli equations.
$$x^2y'+2y=2e^{1/x}y^{1/2}$$
    
<font color='Green'><b>Solution</b></font>:

Let $y=ux$. Then, 

\begin{align*}
& u'x+u={u^3+2u^2+u+1\over(u+1)^2}={u(u+1)^2+1\over(u+1)^2} = u+{1\over(u+1)^2},\\
\Rightarrow \quad & (u+1)^2u'=\frac{1}{x},\\
\Rightarrow \quad & \frac{(u+1)^3}{3}=\ln|x|+c, \quad c \in \mathbb{R},\\
\Rightarrow \quad & (u+1)^3=3(\ln|x|+c), \quad c \in \mathbb{R},\\
\text{Since}~y=ux \quad \Rightarrow \quad & \left({y\over x}+1\right)^3=3(\ln|x|+c), \quad c \in \mathbb{R},\\
\Rightarrow \quad & (y+x)^3=3x^3(\ln|x|+c), \quad c \in \mathbb{R}.
\end{align*}



***

2. Find a function $y_1$ such that the substitution $y=uy_1$ transforms
\begin{align*}y'=\dfrac{y^2+y\tan x+\tan^2 x}{\sin^2x}\end{align*}
into a separable equation. Then solve the equation explicitly. 

**Hint**: Let $y_1=\tan x$.
    
<font color='Green'><b>Solution</b></font>:

Let $y=u\tan(x)$. Then, 

\begin{align*}
& u'\tan (x)+u\sec^2x=(u^2+u+1)\sec^2x,\\
\Rightarrow \quad & u'\tan (x)=(u^2+1)\sec^2x,\\
\Rightarrow \quad & {u'\over u^2+1}=\sec^2(x)\cot (x)=\cot(x)+\tan(x),\\
\Rightarrow \quad & \tan^{-1}u=\ln|\sin (x)|-\ln|\cos (x)|+c=\ln|\tan (x)|+c, \quad c \in \mathbb{R},\\
\Rightarrow \quad & u=\tan(\ln|\tan (x)|+c), \quad c \in \mathbb{R},\\
\end{align*}

As $y=u\tan(x)$,
\begin{align*}y=\tan (x)\ \tan(\ln|\tan (x)|+c), \quad c \in \mathbb{R}.\end{align*}
***

3. Determine whether if the following equation is exact, and then solve it.
$$(3y\cos x+4xe^x+2x^2e^x)\,dx+(3\sin x+3)\,dy=0.$$

<font color='Green'><b>Solution</b></font>:
First off, let $M(x,y)=3y\cos x+4xe^x+2x^2e^x$ and $N(x,y)=3\sin x+3$. Then, we need to show that
\begin{align*}
\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}.
\end{align*}

We have,
\begin{align*}
\frac{\partial M}{\partial y} = 3\cos x= \frac{\partial N}{\partial x}.
\end{align*}
Therefore, the  equation is exact.

Now, to solve this exact equation. We need to identify $F(x,y) = c$ such that
* $\frac{\partial F}{\partial x} = M(x,y)$,
* $\frac{\partial F}{\partial y} = N(x,y)$.

It follows from $\frac{\partial F}{\partial y} = N(x,y)$ that

\begin{align*}
& F(x,y) = \int \left( 3y\cos x+4xe^x+2x^2e^x \right) dy,\\
\Rightarrow \quad & F(x,y) = 3y\sin x+3y+\psi(x).
\end{align*}

Now, to find $\psi(x)$, we can use $\frac{\partial F}{\partial x} = M(x,y)$. This means,

\begin{align*}
& \frac{\partial F}{\partial x} = M(x,y),\\
\Rightarrow \quad & 3y\cos x+\psi'(x) = 3y\cos x+4xe^x+2x^2e^x.
\end{align*}

It follows that
$$\psi'(x)=4xe^x+2x^2e^x.$$
and integration by parts yields
\begin{align*}
\psi(x)=2x^2e^x
\end{align*}
Therefore, 
$F(x,y)=3y\sin x+3y+2x^2e^x$.
and
\begin{align*}3y\sin x+3y+2x^2e^x=c, \quad c \in \mathbb{R}.\end{align*}

***
**Refrences**

1. Trench, William F. "Elementary differential equations with boundary value problems." (2018).
***