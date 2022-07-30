# Numerical Integration

Content:
* Trapezoidal rule
* Simpsons_rule
* Midpoint rule
* Gaussian quadrature


In many practical applications, an approximation of the integral of some functions is needed. In many cases, the definite integral of some functions is not possible as the antiderivatives of these functions are not easy to obtain.

The numerical integration methods that we review here are all based on 
The methods of quadrature in this section are all based on numerical quadratures. 

In the methods of quadrature, a set of distinct nodes \${x_0, \ldots, x_n\}$ from an interval [a, b] is selected, and then the integrate is approximated utilizing the Lagrange interpolating polynomial [2]:

\begin{align*}
L(x)=\sum _{j=0}^{n}y_{j}L_{j}(x)
\end{align*}

Moreover, letting
\begin{align*}
a_{i}=\int_{a}^{b}L_{j}(x)dx
\end{align*}
the quadrature formula is defined as follows,
\begin{align*}
\int_{a}^{b}f(x)\,dx \approx \sum _{j=0}^{n}a_{i}f(x_{i}).
\end{align*}

The error of these approximation is given by [2]
\begin{align*}
\text{Error }(f) = \frac{1}{(n+1)!}
\int_{a}^{b} \prod_{i=1}^{n} (x- x_{i}) f^{n+1} (\xi(x)) \,dx
\end{align*}
where $\xi(x) \in [a, b]$.