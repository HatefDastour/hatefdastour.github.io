# Interpolation and Polynomial Approximation

```{tableofcontents}
```

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Polynomial and the Degree of the Polynomial
</b></font>

An expression of the form $a_nx^n+a_{n-1}x^{n-1}+a_{n-2}x^{n-2}+\ldots+a_{1}x^{1}+a_0$ is called a **polynomial**. In this expression
$a_{0},~a_{1},~\ldots,~a_{n}$ are numbers and $x$ is a variable. If the coeficient of $x^n$ is nonzero ($a_n \neq 0$), the integer
$n$ is called the **degree of the polynomial**, and $a_n$ is called the leading coefficient.
</div>

|                             |                                                              |
|-----------------------------|--------------------------------------------------------------|
|  A polynomial of degree $1$ |                            $ax+b$                            |
| A polynomial of degree  $2$ |                          $ax^2+bx+c$                         |
| A polynomial of degree  $3$ |                       $ax^3+bx^2+cx+d$                       |
|           $\vdots$          |                           $\vdots$                           |
|  A polynomial of degree $n$ | $a_nx^n+a_{n-1}x^{n-1}+a_{n-2}x^{n-2}+\ldots+a_{1}x^{1}+a_0$ |


```{admonition} Weierstrass Approximation Theorem

Let $f\in C[a,b]$. Then for each $\varepsilon>0$, there is a polynomial
$P(x)$ such that
\begin{align*}
|f (x) − P(x)| < \varepsilon,\quad x\in[a,b].
\end{align*}
```

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Interpolating Polynomial
</b></font>

Assume that $n$ data pairs $(x_1,y_1 )$, $(x_2 , y_2 )$, ..., $(x_n , y_n )$ are available in a way that the $x_i$ are distinct. Then, there exists a unique polynomial
\begin{equation*}
p(x) = r_0 +r_1 x+r_2 x^2 +\ldots+r_{n-1} x^{n-1}
\end{equation*}
such that $p(x_i ) = y_i$ for each $i = 1, 2, \ldots, n$.

For this data, this polynomial is called the **interpolating polynomial**.
</div>


***
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***