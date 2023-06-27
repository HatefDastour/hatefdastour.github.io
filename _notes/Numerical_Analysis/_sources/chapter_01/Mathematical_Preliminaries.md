# Mathematical Preliminaries

## Limits and Continuity

`````{admonition} Limit of a function
:class: important


Let's consider a function $f$ defined on a set of real numbers $X$. We say that $f$ has a **limit** $L$ at the point $x_0\in X$ if, for any positive value $\varepsilon$, there exists a real number $\delta > 0$ such that the following condition is satisfied:

\begin{equation}
|f(x_{0}) - L| < \varepsilon
\end{equation}

whenever $0 < |x - x_{0}| < \delta$ for all $x\in X$. In other words, as $x$ approaches $x_0$, the values of $f(x)$ get arbitrarily close to $L$. We represent this limit as:

\begin{equation}
\lim_{n \to x_{0}} f(x) = L
\end{equation}

<iframe src="https://www.geogebra.org/classic/dscrvn3q?embed" width="600" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

`````

`````{admonition} Continuous functions
:class: important

Let's assume that a function $f$ is defined on a set of real numbers $X$. We say that function $f$ is \textbf{continuous} at a specific point $x_0$ if, according to {cite:ps}`burden2005numerical`,
\begin{equation}
\lim_{x \to x_{0}} f (x) = f (x_{0}).
\end{equation}
Furthermore, if the function $f$ is continuous at every point in the set $X$, it is considered to be continuous on the entire set $X."

`````

`````{admonition} Remark
:class: tip

* The set of all natural numbers: $\mathbb{N}$.

* The set of all integer numbers: $\mathbb{N}$.

* The set of all rational numbers: $\mathbb{R}$.

* The set of all real numbers: $\mathbb{R}$.

* The set of all complex numbers: $\mathbb{C}$.

* $\mathbb{N} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R} \subset \mathbb{C}$.

* The set of all functions continuous on interval $[a, b]$: $C[a, b]$.

* The set of all functions continuous on interval [a, b] if their derivatives are also continuous on interval $[a, b]$: $C^2[a, b]$.

* In general, $C^{n}$ means the nth derivative is continuous.

* The set of all functions continuous on $\mathbb{R}$: $C(\mathbb{R})$ or $C(-\infty, \infty)$. 

`````

`````{admonition} Limit of a sequence
:class: important

A sequence of real numbers can be defined as an ordered set of real numbers, denoted as ${x_0,x_1,x_2,\ldots}$ and represented as $\{x_n\}_{n=1}^{\infty}$. According to {cite:ps}`burden2005numerical`, this sequence is said to converge to a point $x$ if, for any positive arbitrary number $\varepsilon$, there exists an integer $N\varepsilon$ such that
\begin{equation}
|x_n - x| < \varepsilon,
\end{equation}
holds for all $n > N_\varepsilon$. In mathematical notation, the convergence of the sequence $\{x_n\}_{n=1}^{\infty}$ to the point $x$ is represented as
\begin{equation}
\lim_{n \to \infty} x_n = x.
\end{equation}
`````

```{admonition} Theorem
Assume that function $f$ is defined on a set of real numbers $X$ and for some values $x_{0} \in X$, $f$ is continuous at point $x_{0}$ if only if any sequence $\{x_n\}_{n=1}^{\infty}$ converges to point $x_{0}$ and
\begin{align*}
\lim_{n \to \infty} f(x_n) = f(x_{0}).
\end{align*}
```

## Differentiability

`````{admonition} Differentiability
:class: important

Let's consider a function $f$ defined on an open interval $(a, b)$ that contains a point $x_{0}$. We can determine if the function is differentiable at $x_{0}$ by checking the existence of the following limit {cite:ps}`burden2005numerical`:

\begin{equation}
f'(x_{0})=\lim_{x\to x_{0}} \frac{f(x)-f(x_{0})}{x - x_{0}}.
\end{equation}

If this limit exists, it implies that the function $f$ is differentiable at the point $x_{0}$. In this context, $f'(x_{0})$ represents the derivative of the function $f$ at the specific point $x_{0}$.

<iframe src="https://www.geogebra.org/classic/qcunx4nc?embed" width="600" height="500" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

`````

`````{admonition} Remark
:class: tip

* A function $f$ is differentiable at point $x_{0}$ if $f'(x_{0})$ exists.
* $f$ is continuous at point $x_{0}$ if the function $f$ is differentiable at at point $x_{0}$.
`````

The following theorem is **Theorem 1.7** from {cite:ps}`burden2005numerical`.

```{admonition} Rolle's Theorem

Let's consider a function $f$ that is continuous on a closed interval $[a, b]$ and differentiable on the open interval $(a, b)$. If the values of $f$ at the endpoints of the interval are equal, i.e., $f(a) = f(b)$, then there must exist a point $c$ within the open interval $(a, b)$ such that the derivative of $f$ at that point, denoted by $f'(c)$, equals zero.

In other words, if $f(a) = f(b)$ under the given conditions, we can conclude that there exists at least one point $c$ in the open interval $(a, b)$ where the derivative of the function $f$ is zero.

<iframe src="https://www.geogebra.org/classic/afngnve8?embed" width="600" height="350" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

```
The following theorem is **Theorem 1.8** from {cite:ps}`burden2005numerical`.

```{admonition} Mean Value Theorem

Let's consider a function $f$ that is continuous on the closed interval $[a, b]$ and differentiable on the open interval $(a, b)$. Suppose there exists a point $c$ in the open interval $(a, b)$ such that the following equality holds:

\begin{equation}
f'(c) = \frac{f(b) - f(a)}{b - a}
\end{equation}

<iframe src="https://www.geogebra.org/classic/g6vcjns6?embed" width="600" height="400" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

```

The following theorem is **Theorem 1.9** from {cite:ps}`burden2005numerical`.

```{admonition} Extreme Value Theorem

Consider a function $f$ that is continuous on the closed interval $[a, b]$. In this case, we can assert the existence of two points $c_1$ and $c_2$ within the interval $[a, b]$ such that for any $x$ in the interval $[a, b]$, the following inequality holds:

\begin{equation}
f(c_1) \leq f(x) \leq f(c_2)
\end{equation}

Thus, we can establish that there exist points $c_1$ and $c_2$ in the closed interval $[a, b]$ for which the function $f$ attains its minimum and maximum values, respectively.

<iframe src="https://www.geogebra.org/classic/ahgw2ucr?embed" width="600" height="400" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

```

The following theorem is **Theorem 1.11** from {cite:ps}`burden2005numerical`.

```{admonition} Intermediate Value Theorem

Let's consider a function $f$ that is continuous on the closed interval $[a, b]$. Suppose there is a number $K$ such that the following inequality holds:

\begin{equation}
f(a) \leq K \leq f(b)
\end{equation}

In such a case, we can conclude that there exists a point $c$ in the open interval $(a, b)$ for which the function $f$ attains the value $K$, satisfying the equation:

\begin{equation}
f(c) = K
\end{equation}

Thus, within the interval $(a, b)$, there exists at least one point $c$ where the function $f$ reaches the value $K$ that lies between $f(a)$ and $f(b)$.

<iframe src="https://www.geogebra.org/classic/xrsayaps?embed" width="600" height="350" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

```

## Integration

`````{admonition} Riemann integral
:class: important

Let's consider a function $f$ defined on a closed interval $[a, b]$ and a sequence of points $x_{0}$, $x_{1}$, $\ldots$, $x_{n}$ satisfying the following conditions:

\begin{equation}
a \leq x_{0} \leq x_{1}\leq \ldots \leq x_{n} =b.
\end{equation}
The Riemann integral of the function $f$ over the interval $[a, b]$ can be computed as the limit of the following expression, provided that the limit exists:

\begin{equation}
\int_{a}^{b} f(x) dx = \lim_{\Delta x_{j} \to 0} \sum_{j = 1}^{n} f(z_{j}) \Delta x_{j}
\end{equation}
where $\Delta x_{j}  = x_{j} -x_{j-1}$ for $j \in \{1, 2,\ldots, n\}$ and $z_{j} \in [x_{j-1}, x_{j}]$.

In this expression, $\Delta x_j = x_j - x_{j-1}$ for $j \in {1, 2, \ldots, n}$ represents the length of each subinterval, and $z_j$ is a point chosen from the interval $[x_{j-1}, x_j]$. The Riemann integral is obtained by taking the limit as the lengths of the subintervals, represented by $\Delta x_j$, approach zero.

`````

`````{admonition} Riemann integral (Equally Spaced)
:class: important

Suppose we have a function $f$ that belongs to the set of continuous functions $C[a, b]$. We can also assume that this function is Riemann integrable on the closed interval $[a, b]$. Additionally, let $x_i$ for $i = 1, 2, \ldots, n$ be equally spaced points within the interval $[a, b]$ with a spacing of $\Delta x = \frac{b-a}{n}$.

In this context, the Riemann integral of $f$ over the interval $[a, b]$ can be computed using the following limit expression:

\begin{equation}
\int_{a}^{b} f(x) dx = \lim_{n \to \infty}\frac{b-a}{n} \sum_{n = 1}^{n} f(x_{j})
\end{equation}

Here, as $n$ approaches infinity, $\frac{b-a}{n}$ represents the width of each subinterval, and the sum $\sum_{j=1}^{n} f(x_{j})$ calculates the value of the function $f$ at each equally spaced point $x_j$. By taking the limit as $n$ tends to infinity, we arrive at the Riemann integral of $f$ over the interval $[a, b]$.

`````

The following theorem is **Theorem 1.13** from {cite:ps}`burden2005numerical`.

```{admonition} Weighted Mean Value Theorem for Integrals

Let's assume that $f$ is a Riemann integrable function that is continuous on the closed interval $[a, b]$. According to a theorem, there exists a point $c$ in the open interval $(a, b)$ such that the following equation holds:

\begin{equation}
\int_{a}^{b} f(x)g(x)\, dx = f(c)\int_{a}^{b} f(x) dx.
\end{equation}

This theorem implies that for any given function $g(x)$, the integral of the product $f(x)g(x)$ over the interval $[a, b]$ can be expressed as the product of the value of $f(c)$ at some point $c$ in $(a, b)$ and the integral of $f(x)$ over the same interval $[a, b]$.

It is important to note that the theorem guarantees the existence of such a point $c$ that satisfies the equation, but it does not provide a specific method to determine the value of $c$.

```

```{admonition} Mean Value Theorem for Integrals

Consider a continuous function $f(x)$ defined over an interval $[a,~b]$. In this case, there exists (at least) a point $c$ within the interval $[a,~b]$ such that {cite:ps}`strang2016calculus`

\begin{equation}
f(c) = \frac{1}{b-a}\int_{a}^{b} f(x)\ dx.
\end{equation}
The above can be also formulated as follows,
\begin{equation}
\int_{a}^{b} f(x)\ dx = f(c)(b-a).
\end{equation}

```

## Taylor Polynomials and Series

`````{admonition} Taylor series, Maclaurin series,  and Maclaurin polynomial
:class: important

Let us assume that $f$ is a function belonging to the class $C^n[a, b]$, where $n$ denotes the number of continuous derivatives of the function $f$ on the interval $[a, b]$. The notation $f^{(n)}$ represents the $n$th derivative of $f$. If $f^{(n)}$ exists on the interval $[a, b]$, then for any $x$ within this interval, there exists a point $x_0$ such that $x_0 \leq \xi(x) \leq x$. This point $x_0$ satisfies the following expression:

\begin{equation}\label{Taylor_App}
f(x) = \underbrace{\sum_{j = 0}^{n} \frac{f^{(j)}(x_{0})}{j!} (x - x_{0})^{j} }_{P_{n}(x):~\text{nth Taylor polynomial}} +
\underbrace{\frac{f^{(n+1)} (\xi(x))}{(n+1)!} {(x - x_{0})^{n+1}}}_{R_{n}(x):~\text{truncation error}}
\end{equation}

Here, we have an equation that relates $f(x)$ to the nth Taylor polynomial $P_n(x)$ and the truncation error $R_n(x)$. The nth Taylor polynomial $P_n(x)$ is defined as the sum of terms from $j = 0$ to $n$, where each term involves the $j$th derivative of $f$ evaluated at $x_0$, divided by $j!$, multiplied by $(x - x_0)^j$. On the other hand, the truncation error $R_n(x)$ involves the $(n+1)$th derivative of $f$ evaluated at some point $\xi(x)$ between $x_0$ and $x$, divided by $(n+1)!$, multiplied by $(x - x_0)^{n+1}$.

By taking the limit of $P_n(x)$ as $n$ approaches infinity, we obtain an infinite series known as the **Taylor series** for $f$ centered around $x_0$. When $x_0 = 0$, this series is specifically referred to as the **Maclaurin series**. In the case of the Maclaurin series, the nth Maclaurin polynomial $P_n(0)$ serves as an approximation of $f(0)$ within the given interval.

`````

`````{admonition} Remark: Mean-value forms of the remainder
:class: tip

Assume that $f : \mathbb{R} \rightarrow \mathbb{R}$ be $k + 1$ times differentiable on the open interval and $f^{(k)}$ is continuous on the closed interval between $a$ and $x$ \cite{apostol1991calculus}. Then

```{math}
:label: Taylor_remainder
R_{k}(x)={\frac {f^{(k+1)}(\xi)}{(k+1)!}}(x-a)^{k+1}
```

for some real number $\xi$ between $a$ and $x$. This $R_{k}(x)$ from equation {eq}`Taylor_remainder` is also known as the Lagrange form of the remainder {cite:ps}`hirschman2014infinite`.
`````
<font color='Blue'><b>Example</b></font>: Let $f (x) = \sin (x)$ and $x_0 = 0$. Determine the Taylor polynomial for $f$ about $x_0 = 0$ for any given values on $n\in \mathbb{N}$.

<font color='Green'><b>Solution</b></font>:
First of all, $\sin(x) \in C^{\infty}(\mathbb{R})$ for $x\in \mathbb{R}$. Moreover,

\begin{equation*}
\begin{array}{lcl}
f(x) = \sin(x) & \Rightarrow & f(0) = 0   ,\\
f'(x)  =  \cos(x) & \Rightarrow & f'(0) = 1   ,\\
f''(x)  =  -\sin(x) & \Rightarrow & f''(0) =0   ,\\
f'''(x)  = -\cos(x) & \Rightarrow & f'''(0) = -1   ,\\
f^{(4)}(x)  =  \sin(x) & \Rightarrow & f^{(4)}(0) =0   ,\\
f^{(5)}(x)  =  \cos(x) & \Rightarrow & f^{(5)}(0) = 1   ,\\
\vdots & & \vdots
\end{array}
\end{equation*}
Therefore,
\begin{align*}
P_{n}(x) &= f(0) + \frac{1}{1!} f'(0)\,x + \frac{1}{2!}f''(0)\,x^{2} + \frac{1}{3!}f'''(0)\,x^{3} + \frac{1}{4!}f^{(4)}(0)\,x^{4} + \ldots
\notag \\ &
= \frac{1}{1!}(1)\,x + \frac{1}{3!}(-1)\,x^{3} + \frac{1}{5!}(1)\,x^{5} + \ldots
\notag \\ &
= \frac{(-1)^{0}}{(2(0) +1)!}x^{2(0)+1} +  \frac{(-1)^{1}}{(2(1) +1)!}x^{2(1)+1}
+  \frac{(-1)^{2}}{(2(2) +1)!}x^{2(2)+1}
+ \ldots
\notag \\ &
= \sum_{j = 0}^{n} \frac{(-1)^{j}}{(2j +1)!}x^{2j+1}
\end{align*}