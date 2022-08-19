# Algorithms and Convergence

## Algorithms

An **algorithm** is a procedure that applies a finite number of operations on some inputs to produce some outputs. **Pseudocodes** and **flowcharts** are often used to describe algorithms. 

For example, in pseudocodes, we often use

* **Looping techniques** such as **For** and **While** loops:

```
For i = 1, 2, . . . , n
    do something
	
While i < N
    do something
    i = i + 1
```

* **Condition-controlled** statements: **If**, **Else If**, **Else**,...

```
If Some-Condition
    do something
Else If Some-Other-Condition
    do something else
Else
    something different from the previous two
```
   
<font color='Blue'><b>Example</b></font>: Write down an algorithm that generates $\sum_{i = 1}^{N} \sin(x_{i})$ for given values of $x_{1}$, $x_{2}$, $\ldots$, $x_{n}$.

<font color='Green'><b>Solution</b></font>:

 ``` 
INPUT: N, x1, x2, . . . , xN.
OUTPUT SUM of sin(xi) for i = 1,2,..., N
i=1 xi.
Step 1: Set SUM = 0. ( Initialize accumulator.)
Step 2:
For i = 1, 2, . . . , N do
    set SUM = SUM + sin(xi). ( Add the next term.)
Step 3: OUTPUT (SUM);
STOP.
```

For generating a flowchart, we need to pay attention to the meaning of each shape. Generally, there is a rounded edge rectangular shape for start/end, rectangular for process, Rhombus shape for decision, and arrows for connecting them. Please see [this page](https://support.microsoft.com/en-us/office/create-a-basic-flowchart-in-visio-e207d975-4a51-4bfa-a356-eeec314bd276) for more details.

For the above algorithm, we have,

```{figure} ../Figs/Flowchart_Example.png
---
height: 600px
---
Flowchart Example
```

## Order of Convergence

```{admonition} Theorem: Order of Convergence

Assume that $\{c_{n}\}$ is a sequence of approximate solutions that converge to a point $c$. Let $c_{n} \neq c$ for $n\in \mathbb{N}$, then there exists $\lambda$ and $\alpha$ such that
\begin{align*}
\lim_{n \to \infty} \frac{\|c_{n+1} - c\|}{\|c_{n} - c\|^{\alpha}} = \lambda
\end{align*}
where $\|.\|$ is a distance function (such as absolute value for real values). Then, $\alpha$ represents the order of convergence while $\lambda$ is an asymptotic error constant.

```

`````{admonition} Remark
:class: tip

In the previous theorem,

* If $\alpha = 1$ (and $\lambda <1$), the $\{c_{n}\}$ is **linearly convergent**.
* If $\alpha = 2$ (and $\lambda <1$), the $\{c_{n}\}$ is **quadratically convergent**.
* If $\alpha = 3$ (and $\lambda <1$), the $\{c_{n}\}$ is **cubically convergent** (cubic convergence).
* Etc.
`````

## Big O Notation

Big $\mathcal{O}$ is a notion that measures the convergence rate of an algorithm and its rate of error. Big $\mathcal{O}$ can be used for describing an error term. For example, the Taylor series of $e^{x}$ can be found as follows,

\begin{align*}
e^{x} = 1+x+ \frac {x^{2}}{2!} + \frac {x^{3}}{3!} + \frac {x^{4}}{4!} +\ldots
\end{align*}
Then, for example, when $x$ is approaching zero,
\begin{align*}
e^{x} = 1+x+ \frac {x^{2}}{2!} + \frac {x^{3}}{3!} + \mathcal{O}(x^4)
\end{align*}
means the following absolute error
\begin{align*}
\left| e^{x} - (1+x+ \frac {x^{2}}{2!} + \frac {x^{3}}{3!}) \right| = \mathcal{O}(x^4)
\end{align*}
is almost a constant times $x^4$ when $x$ is getting closer to zero.


Another usage of this would be analyzing how efficient an algorithm is. For example, $f(x) = x^3 + 2\,x^2 + x$
has a Big $\mathcal{O}$ growth rate $\mathcal{O}(x^3)$ and Big $\mathcal{O}$ decline rate of $\mathcal{O}(x)$.

***
**References:**
1. Burden, Richard L., and J. Douglas Faires. "Numerical analysis 8th ed." Thomson Brooks/Cole (2005).
1. Atkinson, Kendall E. An introduction to numerical analysis. John wiley & sons, 2008.
1. Khoury, Richard, and Douglas Wilhelm Harder. Numerical methods and modelling for engineering. Springer, 2016.
***