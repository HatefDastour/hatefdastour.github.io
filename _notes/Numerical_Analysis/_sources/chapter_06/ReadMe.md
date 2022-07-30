# Initial-Value Problems for Ordinary Differential Equations

Content:
* First-order methods
	* Forward Euler method
	* Backward Euler method
* Second-order methods
	* Heun’s method method
	* Trapezoidal rule
	* Midpoint methods
	* Second Runge-Kutta methods
* Higher-order methods
	* Third Runge-Kutta methods
	* Fourth Runge-Kutta methods


In this section, we go through several methods that can approximate the solution of a well-posed initial-value problem (IVP) on grid points. Consider the following IVP:

\begin{align*}
\frac{dy}{dt} &= f(t,y),& a \leq t \leq b,~y(a) = y_{0}.
\end{align*}

Here it is assumed that the grid points are equally distributed throughout
the interval $[a, b]$. Let $N$ be a positive integer, we have, the following step size

\begin{align*}
h = \Delta t = \frac{b-a}{N}
\end{align*}
and each grid point can be identified as
\begin{align*}
t_{j} &= a +jh,& j = 0,1,2,\ldots,N.
\end{align*}

Moreover, let $y_{j}$ denote approximation $y$ at grid points for $j = 1,2,3,\ldots,N$, we can use several methods.