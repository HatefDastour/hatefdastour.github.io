# Introduction

```{tableofcontents}
```

A differential equation is a mathematical expression including one or more derivatives of an unknown function. A differential equation's order is determined by the highest derivative it includes. If a differential equation involves an unknown function of just one variable, it is called an ordinary differential equation; if it comprises partial derivatives of more than one variable, it is called a partial differential equation. For the time being, we will just discuss ordinary differential equations, which we will simply refer to as differential equations {cite:ps}`barbu2016differential, trench2001elementary`.

First-order differential equations of the type are the simplest differential equations, and they can be expressed in the following form  {cite:ps}`barbu2016differential, trench2001elementary`
```{math}
:label: eq:1.2.1
\frac{dy}{dt}=f(t) \mbox{\quad or, equivalently, \quad}y'=f(t),
```

$f$ is a known function of $t$. We learned how to identify functions that satisfy this sort of problem in Calculus and Differential Equation classes.

<font color='Blue'><b>Example</b></font>:
For example, if
\begin{equation*}
y'=t^3,
\end{equation*}
then
\begin{equation*}
y=\int t^3\, dt=\frac{t^4}{4}+c,
\end{equation*}
where $c$ is an arbitrary constant.

It is not necessary to study differential equations like {eq}`eq:1.2.1` except for illustration reasons in this section. We'll generally look at differential equations that look like this:

\begin{equation} \label{eq:1.2.2}
y^{(n)}=f(t,y,y', \dots,y^{(n-1)}),
\end{equation}
where at least one of the functions $y$, $y'$, \dots, $y^{(n-1)}$ occurs on the right {cite:ps}`trench2001elementary`.

<font color='Blue'><b>Examples</b></font>:
\begin{align*}
\begin{array}{rcll}
\displaystyle{dy\over dt} - t^2&=&0&\mbox{(first order)},\\
\displaystyle{dy\over dt}+3ty^3&=&-2&\mbox{(first order)},\\
\displaystyle{d^2y\over dt^2}+2\displaystyle{dy\over dt}+y&=&4t&\mbox{(second order)},\\
ty'''+y^2&=&\sin(t)  &\mbox{(third order)},\\
y^{(n)}+ty'+3y&=&t&\mbox{($n$-th order)}.
\end{array}
\end{align*}