# 1.1 Systems of Equations, Geometry

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Linear Equation
</b></font>

Let $a$, $b$, and $c$ be real numbers ($a$ and $b$ are not both zero). Then, the graph of an equation with the following form
\begin{equation*}
ax+by = c
\end{equation*}
is a straight line. Such an equation is called a **linear equation**, and the **variables** of this linear equation are $x$ and $y$.
</div>

For example, $x-y=0$ is a linear equation.

<center>
<iframe src="https://www.desmos.com/calculator/64mqn7hni9?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>
</center>

Note that, here, $x$ and $y$ are the variables. However, in general, when more than two variables are involved, variables are often demonstrated with some subscripts. For example, $x_1$, $x_2$, ..., $x_n$ are variables for an equation of the form
\begin{equation*}
a_1 x_1 +a_2 x_2 +\ldots+a_n x_n = b
\end{equation*}

Moreover, $\Sigma$ (Sigma) is often used to demonstrate a sum of some terms. For example,
\begin{equation*}
a_1 x_1 +a_2 x_2 +\ldots+a_n x_n = b
\end{equation*}
also can be shows as follows
\begin{equation*}
\sum_{j = 1}^{n}  a_j\,x_j  = b
\end{equation*}
which shows a sumation of $n$ terms. This also know as **summation notation**.


<div class="alert alert-info" role="alert">
<font size="+1"><b>
System of Linear Equations
</b></font>

A system of equations is a collection of equations. For example, for linear equations $a_{11}x_1+\ldots+a_{1n}x_{n}=b_1$, $a_{21}x_1+\ldots+a_{2n}x_{n}=b_2$, $\ldots$, $a_{m1}x_1+\ldots+a_{mn}x_{n}=b_m$.

\begin{align*}
\begin{cases}
a_{11}x_1+\ldots+a_{1n}x_{n}=b_1\\
a_{21}x_1+\ldots+a_{2n}x_{n}=b_2\\
\vdots \\
a_{m1}x_1+\ldots+a_{mn}x_{n}=b_m.
\end{cases}
\end{align*} 
</div>

In terms of summation notation, the above linear equation can be written as
\begin{align*}
\sum_{j = 1}^{n}  a_{ij}\,x_{ij}  = b_{i},\quad i = 1, 2, 3, \ldots, m.
\end{align*} 

<font color='Blue'><b>Example</b></font>:
The following system of equation,

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


<div class="alert alert-info" role="alert">
<font size="+1"><b>
Homogeneous System of Equations
</b></font>
<p style='text-align: justify;'>
A system of equations is called homogeneous if all the right hand side values are zero (each equation in the system is equal to zero).
</p>
</div>

<font color='Blue'><b>Example</b></font>:
The system of equation,
\begin{align*}
\begin{cases}
x+y=0\\
x-y=0,\\
\end{cases}
\end{align*}
is homogeneous.


<div class="alert alert-info" role="alert">
<font size="+1"><b>
Solution of a Linear System
</b></font>
If $(x_1,~x_2,~x_3,\ldots,~x_n)$ is a solution for a linear system, then it satisfies every equation of that linear system.
</div>

<font color='Blue'><b>Example</b></font>:
Show that $x = -2$, $y = 5$, $z = 0$ and $x = 0$, $y = 4$, $z = -1$ are
both solutions to the system, 
\begin{align*}
\begin{cases}
x+y+ z=3,\\
2x+y+3z=1.
\end{cases}
\end{align*}

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
***

## 1.1.1 Possible sets of solution for two equations and two variables

When a system of linear equations has only two variables, then the solutions to that system of linear equations can be explained geometrically using a graph. The graph of an equation $ax+by = c$ is a straight line when $a$ and $b$ are not both zero at the same time.

For the following system of linear equations (with two variables), there are three possibilities.

\begin{align*}
\begin{cases}
a_{11}x+a_{12}y=b_1\\
a_{21}x+a_{22}y=b_2\\
\end{cases}
\end{align*} 

Note that each equation can be shown on a graph using a straight line, and there are three possibilities for the
corresponding straight lines:

1.  The lines intersect at a only one point. Then the system has a **unique solution** corresponding to that point.

<font color='Blue'><b>Example</b></font>: For the following system of linear equations,
\begin{align*}
\begin{cases}
x + y = 2\\
x - y = -1\\
\end{cases}
\end{align*} 
we have,

<center>
<iframe src="https://www.desmos.com/calculator/vnw7ffhpe1?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>
</center>

As can be seen, $(x, y) = (0.5, 1.5)$ is a solution. In this case, it's the only solution (unique solution).

2.  The lines are parallel (and distinct) and so do not intersect. Then the system has **no solution**.

<font color='Blue'><b>Example</b></font>: For the following system of linear equations,
\begin{align*}
\begin{cases}
x + y = 2\\
x + y = -1\\
\end{cases}
\end{align*} 
we have,

<center>
<iframe src="https://www.desmos.com/calculator/xzutr6yr9u?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>
</center>

The two lines are parallel and there is no solution.

3.  The lines are identical. Then the system has infinitely many solutions.

<font color='Blue'><b>Example</b></font>: For the following system of linear equations,
\begin{align*}
\begin{cases}
2\,x + 2\,y = 2\\
x + y = 1\\
\end{cases}
\end{align*} 
we have,

<center>
<iframe src="https://www.desmos.com/calculator/vtceot3sfb?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>
</center>

## 1.1.2 Consistent and inconsistent linear systems

A system of equations is called **inconsistent** when there is no solution for this system of equations, and it is called **consistent** when there is at least one solution for it.

The graph of $ax+by+cz = d$ (it has hree variables) is a plane.

<center>

```{figure} ../Figures/fig1_02.jpg
---
scale: 60%
align: center
---
a) three planes intersecting in a line, b) three planes intersecting in a point, c) three planes with no intersection, d) three planes with no intersection
```

</center>

This graphical method has its limitations. When more than three variables are involved, we can not graph the planes anymore.


***
## Refrences
1. Kuttler, Kenneth. "[A First Course in Linear Algebra (Lyryx)](https://lyryx.com/first-course-linear-algebra/)." (2021).
1. Nicholson, W. Keith. "[Linear Algebra with Applications (Lyryx)](https://lyryx.com/linear-algebra-applications/)." (2021).
***