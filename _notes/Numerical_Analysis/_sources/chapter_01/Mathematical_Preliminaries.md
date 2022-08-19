# Mathematical Preliminaries

## Limits and Continuity

**Limit of a function:**
Assume that function $f$ is defined on a set of real numbers $X$. If for any positive arbitrary number $\varepsilon$, there is a real number $\delta > 0$ exists such that
\begin{align*}
|f (x) - L| < \varepsilon,
\end{align*}
whenever $0 < |x - x_{0}| < \delta$ for all $x\in X$, the function $f$ has the **limit** $L$ at point $x_0\in X$. This limit of the function $f$, $L$, can be shown as follows,
\begin{align*}
\lim_{n \to x_{0}} f (x) = L.
\end{align*}

<iframe src="https://www.geogebra.org/classic/dscrvn3q?embed" width="600" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

**Continuous functions:**
Assume that function $f$ is defined on a set of real numbers $X$. Function $f$ is **continuous** at point $x_0$ if
\begin{align*}
\lim_{n \to x_{0}} f (x) = f (x_{0}).
\end{align*}

In addition, if the function is continuous on every point from the set $X$, then the function is continuous on the set $X$.

`````{admonition} Remark
:class: tip

* The set of all real numbers: $\mathbb{N}$.

* The set of all real numbers: $\mathbb{R}$.

* The set of all functions continuous on interval $[a, b]$: $C[a, b]$.

* The set of all functions continuous on interval [a, b] if their derivatives are also continuous on interval $[a, b]$: $C^2[a, b]$.

* The set of all functions continuous on $\mathbb{R}$: $C(\mathbb{R})$ or $C(-\infty, \infty)$.

`````

**Limit of a sequence:**
A sequence of real numbers is an ordered set of real numbers $\{x_0,x_1,x_2,\ldots\}$ is shown with $\{x_n\}_{n=1}^{\infty}$. In case, for any positive arbitrary number $\varepsilon$, there is an integer number $N_\varepsilon$ exists such that
\begin{align*}
|x_n - x| < \varepsilon, 
\end{align*}
for all $n>N_\varepsilon$, the sequence$\{x_n\}_{n=1}^{\infty}$ **converges** to a point $x$ 
\begin{align*}
\lim_{n \to \infty} x_n = x.
\end{align*}

```{admonition} Theorem
Assume that function $f$ is defined on a set of real numbers $X$ and for some values $x_{0} \in X$, $f$ is continuous at point $x_{0}$ if only if any sequence $\{x_n\}_{n=1}^{\infty}$ converges to point $x_{0}$ and
\begin{align*}
\lim_{n \to \infty} f(x_n) = f(x_{0}).
\end{align*}
```


## Differentiability

Assume that function $f$ is defined on a open interval $(a, b)$ which includes point $x_{0}$, the function is differentiable at point $x_{0}$ if the following limit exists
\begin{align*}
f'(x_{0})=\lim_{x\to x_{0}} \frac{f(x)-f(x_{0})}{x - x_{0}}.
\end{align*}
In this case, $f'(x_{0})$ denotes the dervative of function $f$ at point $x_{0}$.

<iframe src="https://www.geogebra.org/classic/qcunx4nc?embed" width="600" height="500" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

`````{admonition} Remark
:class: tip

* A function $f$ is differentiable at point $x_{0}$ if $f'(x_{0})$ exists.
* $f$ is continuous at point $x_{0}$ if the function $f$ is differentiable at at point $x_{0}$.
`````


```{admonition} Rolle's Theorem

Assume that function $f$ is continuous on a closed interval $[a,b]$ and it is differentiable on the open interval $(a,b)$, then if $f(a) = f(b)$, there exists a $c\in(a, b)$ such that  $f '(c) = 0$.

<iframe src="https://www.geogebra.org/classic/afngnve8?embed" width="600" height="350" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

```


```{admonition} Mean Value Theorem

Assume that function $f$ is continuous on a closed interval $[a,b]$ and it is differentiable on the open interval $(a,b)$, then if there exists a $c\in(a, b)$ such that
\begin{align*}
f '(c) = \frac{f (b) - f (a)}{b - a}
\end{align*} 

<iframe src="https://www.geogebra.org/classic/g6vcjns6?embed" width="600" height="400" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

```

```{admonition} Extreme Value Theorem

Assume that function $f$ is continuous on a closed interval $[a,b]$, then there exits $c_{1}$ and $c_{2}$ from $[a,b]$ such that 
\begin{align*}
f(c_{1}) \leq f(x) \leq f(c_{2}), \quad x \in [a,b].
\end{align*} 

<iframe src="https://www.geogebra.org/classic/ahgw2ucr?embed" width="600" height="400" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

```

```{admonition} Intermediate Value Theorem

Assume that function $f$ is continuous on a closed interval $[a,b]$, and $K$ is a number such that 
\begin{align*}
f(a) \leq K \leq f(b).
\end{align*} 
Then, there exits $c$ from $(a,b)$ such that 
\begin{align*}
f(c) = K.
\end{align*} 

<iframe src="https://www.geogebra.org/classic/xrsayaps?embed" width="600" height="350" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

```

## Integration

**Riemann integral:**
For a function $f$ and a closed interval $[a, b]$ and points $x_{0}$, $x_{1}$, $\ldots$, $x_{n}$ such that
\begin{align*}
a \leq x_{0} \leq x_{1}\leq \ldots \leq x_{n} =b.
\end{align*}
The function's Riemann integral on the interval can be calculated as the following limit if such limit exists.
\begin{align*}
\int_{a}^{b} f(x) dx = \lim_{\Delta x_{j} \to 0} \sum_{j = 1}^{n} f(z_{j}) \Delta x_{j}
\end{align*}
where $\Delta x_{j}  = x_{j} -x_{j-1}$ for $j \in \{1, 2,\ldots, n\}$ and $z_{j} \in [x_{j-1}, x_{j}]$.

**Riemann integral (Equally Spaced):**

Assume that $f \in C[a,b]$. This function is also Riemann integrable on this closed interval $[a, b]$. Also, let $x_i$ for $i = 1, 2, \ldots , n$ be equally spaced with $\Delta x = \dfrac{b-a}{n}$ in $[a, b]$, then

\begin{align*}
\int_{a}^{b} f(x) dx = \lim_{n \to \infty}\frac{b-a}{n} \sum_{n = 1}^{n} f(x_{j})
\end{align*}

```{admonition} Weighted Mean Value Theorem for Integrals
Assume that $f$ is a Riemann integrable function and is continuous on a closed interval $[a, b]$. There there exists $c\in(a,b)$ such that
\begin{align*}
\int_{a}^{b} f(x)g(x) dx = f(c)\int_{a}^{b} f(x) dx.
\end{align*}
```

## Taylor Polynomials and Series

Assume $f \in C^n[a, b]$ and let $f^{n}$ denotes $n$th derivative of the function $f$. If $f^{n}$ also exists on $[a,b]$, then for any $x$ from the interval $[a,b]$, there exists $x_{0} \leq \xi(x) \leq x$ such that

\begin{align*}
f(x) = \underbrace{\sum_{0 = 1}^{n} \frac{f^{(j)}(x_{0})}{j!} (x - x_{0})^{j} }_{P_{n}(x):~\text{nth Taylor polynomial}} +
\underbrace{\frac{f^{(n+1)} (\xi(x))}{(n+1)!} {(x - x_{0})^{n+1}}}_{R_{n}(x):~\text{truncation error}}
\end{align*} 

Taking the limit of $P_{n}(x)$ as $n \to \infty$ gives an infinite series which is known as **Taylor series** for $f$ about $x_{0}$. Moreover, when $x_{0} = 0$, then the infinite series is called **Maclaurin series** and $P_{n}(0)$ is called **Maclaurin polynomial**.

Note that here $R_{n}$ is the truncation error which is the discrepancy between a real and a truncated value.

<font color='Blue'><b>Example</b></font>: Let $f (x) = \cos (x)$ and $x_0 = 0$. Determine the Taylor polynomial for $f$ about $x_0 = 0$ for any given values on $n\in \mathbb{N}$.

<font color='Green'><b>Solution</b></font>: First of all, $\sin(x) \in C^{\infty}(\mathbb{R})$ for $x\in \mathbb{R}$. Moreover,

\begin{align*}
f'(0) & = \left. \cos(x) \right|_{x_{0}} = 1   ,\\
f''(x) & = \left. -\sin(x)\right|_{x_{0}} = 0   ,\\
f'''(x) & = \left. -\cos(x) \right|_{x_{0}} = -1   ,\\
f^{4}(x) & = \left. \sin(x) \right|_{x_{0}} = 0   ,\\
f^{5}(x) & = \left. \cos(x) \right|_{x_{0}} = 1   ,\\
\vdots &
\end{align*}

Therefore,
\begin{align*}
P_{n}(x) & = \sum_{j = 0}^{n} \frac{(-1)^{j}}{(2j +1)!}x^{2j+1}
\end{align*}


***
**References:**
1. Burden, Richard L., and J. Douglas Faires. "Numerical analysis 8th ed." Thomson Brooks/Cole (2005).
1. Atkinson, Kendall E. An introduction to numerical analysis. John wiley & sons, 2008.
1. Khoury, Richard, and Douglas Wilhelm Harder. Numerical methods and modelling for engineering. Springer, 2016.
***