# Systems of Equations, Geometry

**Linear equation**:
If $a$, $b$, and $c$ are real numbers, the graph of an equation of the form
\begin{equation*}
ax+by = c
\end{equation*}
is a straight line (if $a$ and $b$ are not both zero), so such an equation is called a *linear equation* in the *variables* $x$ and $y$.

For example, $x-y=0$ is a linear equation.

```{image} ../Figures/fig1_00.png
:width: 300px
:align: center
```


In general, when more than two variables are involved, variables are often shown with $x_1$, $x_2$, ..., $x_n$. An equation of the form
\begin{equation*}
a_1 x_1 +a_2 x_2 +\ldots+a_n x_n = b
\end{equation*}
is a linear equation with $n$ variables $x_1$, $x_2$, ..., $x_n$ (here $a_1$, $a_2$, ..., $a_n$ and
$b$ denote real numbers).

**System of linear equations**:
A finite collection of linear equations in the variables $x_1$, $x_2$,
..., $x_n$ is called a *system of linear equations* in these variables.

<font color='Blue'><b>Example</b></font>:
The system of equation,

\begin{align*}
\begin{cases}
x_1-2x_2-7x_3=7\\
-x_1+3x_2+6x_3=25\pi
\end{cases}\end{align*}

is linear and has

-   **Variables** (unknowns): $x_1, x_2$ and $x_3$,

-   **Coefficients** (the first equation): $1, -2$, $-7$,

-   **Coefficients** (the second equation): $-1, 3$, $6$,

-   **Constant term** (the first equation): $7$,

-   **Constant term** (the second equation): $25\pi$.

**Homogeneous System of Equations**: A system of equations is called homogeneous if each equation in the
system is equal to 0 .

<font color='Blue'><b>Example</b></font>: The system of equation, \begin{align*}
\begin{cases}
x+y=0\\
x-y=0,\\
\end{cases}\end{align*} is homogeneous.

**Solution of a linear system**: A solution of a linear system is a point that satisfies every
equation.

Show that $x = -2$, $y = 5$, $z = 0$ and $x = 0$, $y = 4$, $z = -1$ are
both solutions to the system, 
\begin{align*}\begin{cases}
x+y+ z=3,\\
2x+y+3z=1.
\end{cases}\end{align*}

Basically, we need to plug each solution into the system of equation.

* Try $x = -2,~y = 5,~z = 0$

\begin{align*}
\begin{cases}
-2+5+ 0=3\\
2(-2)+5+3(0)=1
\end{cases}
\Rightarrow
\begin{cases}
3=3~\surd\\
1=1~\surd
\end{cases},\end{align*}

* Try $x = 0,~y = 4,~z = -1$

\begin{align*}\begin{cases}
-0+4+ -1=3\\
2(0)+4+3(-1)=1
\end{cases}
\Rightarrow
\begin{cases}
3=3~\surd\\
1=1~\surd
\end{cases},\end{align*}

## Possible sets of solution for two equations and two variables

When only two variables are involved, the solutions to systems of linear equations can be described geometrically because the graph of a linear
equation $ax+by = c$ is a straight line if $a$ and $b$ are not both zero.

If the system has two equations, there are three possibilities for the
corresponding straight lines:

1.  The lines intersect at a single point. Then the system has a unique solution corresponding to that point.

```{image} ../Figures/fig1_01a.png
:width: 200px
:align: center
```

2.  The lines are parallel (and distinct) and so do not intersect. Then the system has no solution.

```{image} ../Figures/fig1_01b.png
:width: 200px
:align: center
```


3.  The lines are identical. Then the system has infinitely many solutions---one for each point on the (common) line.

```{image} ../Figures/fig1_01c.png
:width: 200px
:align: center
```


Check [this link](https://www.desmos.com/calculator/l8vbpfq2u4) for an interactive example.

**Consistent and inconsistent linear systems**: A system that has no solution is called *inconsistent*, and a system
with at least one solution is called *consistent*.

With three variables, the graph of an equation $ax+by+cz = d$ can be shown to be a plane.

```{figure} ../Figures/fig1_02a.png
---
scale: 100%
align: center
---
Three planes intersecting in a line
```

```{figure} ../Figures/fig1_02b.png
---
scale: 100%
align: center
---
Three planes intersecting in a point
```

```{figure} ../Figures/fig1_02c.png
---
scale: 100%
align: center
---
Three planes with no intersection
```

```{figure} ../Figures/fig1_02d.png
---
scale: 100%
align: center
---
Three planes with no intersection
```

However, this graphical method has its limitations: When more than three variables are involved, no physical image of the
graphs is possible. It is necessary to turn to a more “algebraic” method of solution.


***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***