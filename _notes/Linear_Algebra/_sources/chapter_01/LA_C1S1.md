# Systems of Equations, Geometry

`````{admonition} Linear Equation
:class: tip

A linear equation in two variables is expressed as
\begin{align}
ax+by = c
\end{align}
where $a$, $b$, and $c$ are constants, and $a$ and $b$ are not both zero. The graph of such an equation is a line that represents all the points $(x, y)$ satisfying the equation.

`````
Understanding linear equations and their graphs is essential in mathematics, as they play a fundamental role in various applications such as modeling real-world relationships, solving systems of equations, and analyzing geometric shapes and transformations.

For example, $x-y=0$ is a linear equation.

<center>
<iframe src="https://www.desmos.com/calculator/64mqn7hni9?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>
</center>

Note that, here, $x$ and $y$ are the variables. However, in general, when more than two variables are involved, variables are often demonstrated with some subscripts. For example, $x_1$, $x_2$, ..., $x_n$ are variables for an equation of the form

\begin{align}
a_1 x_1 +a_2 x_2 +\ldots+a_n x_n = b
\end{align}

Moreover, $\Sigma$ (Sigma) is often used to demonstrate a sum of some terms. For example,
\begin{align}
a_1 x_1 +a_2 x_2 +\ldots+a_n x_n = b
\end{align}
also can be shown as follows
\begin{align}
\sum_{j = 1}^{n}  a_j\,x_j  = b.
\end{align}
This is also known as **summation notation** (a summation of $n$ terms).


`````{admonition} System of Linear Equations
:class: tip

A **system of equations** is a collection of equations. For instance, the following $m$ equations form a system of (linear) equations:

\begin{align}
\begin{cases}
a_{11}x_1 + \ldots + a_{1n}x_n = b_1 \\
a_{21}x_1 + \ldots + a_{2n}x_n = b_2 \\
\vdots \\
a_{m1}x_1 + \ldots + a_{mn}x_n = b_m \\
\end{cases}
\end{align}

In this system, there are $m$ equations and $n$ variables, $x_1, x_2, \ldots, x_n$. Each equation contains a linear combination of these variables with coefficients $a_{ij}$, and the right-hand side of each equation is given by $b_i$.

`````

Solving a system of equations involves finding the values of the variables $x_1, x_2, \ldots, x_n$ that satisfy all the equations in the system simultaneously. The solution to the system is the set of values for the variables that make each equation true.

Systems of equations have broad applications across various fields, such as engineering, physics, economics, and optimization problems. They are fundamental in understanding and modeling complex relationships and interactions between different variables in real-world scenarios.


Using summation notation, the given linear equation can be expressed as:

\begin{align}
\sum_{j=1}^{n} a_{ij}x_{j} = b_i, \quad i = 1, 2, 3, \ldots, m.
\end{align}

In this notation, $i$ represents the index of each equation in the system (from 1 to $m$), while $j$ represents the index of each variable (from 1 to $n$). The coefficients $a_{ij}$ and the variables $x_j$ are combined in the summation on the left-hand side of each equation. The right-hand side of each equation is represented by $b_i$.

Using summation notation allows us to concisely represent a system of linear equations with multiple variables and equations. It is a powerful mathematical tool that simplifies the expression and makes it easier to work with complex systems of equations.

<font color='Blue'><b>Example</b></font>:
The following system of equations,

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


`````{admonition} Homogeneous System of Equations
:class: tip

A system of equations is called **homogeneous** if all the right-hand side values are zero (each equation in the system is equal to zero). In a homogeneous system, the equations have the following form:

\begin{align}
a_{11}x_1 + a_{12}x_2 + \ldots + a_{1n}x_n &= 0 \\
a_{21}x_1 + a_{22}x_2 + \ldots + a_{2n}x_n &= 0 \\
&\vdots \\
a_{m1}x_1 + a_{m2}x_2 + \ldots + a_{mn}x_n &= 0 \\
\end{align}

where all $b_i$ (right-hand side values) are zero.


`````

Homogeneous systems of equations are of particular interest in linear algebra and have important applications in various areas, such as linear transformations, eigenvalues, and eigenvectors. Solving homogeneous systems often involves finding non-trivial solutions, meaning solutions where not all variables are equal to zero. The existence and properties of non-trivial solutions can provide valuable insights into the behavior of certain mathematical structures and physical phenomena.

<font color='Blue'><b>Example</b></font>:
The system of equations,
\begin{align*}
\begin{cases}
x+y=0\\
x-y=0,\\
\end{cases}
\end{align*}
is homogeneous.


`````{admonition} Solution of a Linear System
:class: tip

If $(x_1, x_2, x_3, \ldots, x_n)$ is a solution for a linear system, it means that when these values are substituted into each equation of the linear system, every equation holds. In other words, the solution satisfies every equation in the linear system.

`````

<font color='Blue'><b>Example</b></font>:
Show that $x = -2$, $y = 5$, $z = 0$ and $x = 0$, $y = 4$, $z = -1$ are
both solutions to the system, 
\begin{align*}
\begin{cases}
x+y+ z=3,\\
2x+y+3z=1.
\end{cases}
\end{align*}

We need to plug each solution into the system of equations.

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

## Possible sets of solutions for two equations and two variables

When a system of linear equations has only two variables, then the solutions to that system of linear equations can be explained geometrically using a graph. The graph of an equation $ax+by = c$ is a straight line when $a$ and $b$ are not both zero at the same time.

For the following system of linear equations (with two variables), there are three possibilities.

\begin{align}
\begin{cases}
a_{11}x+a_{12}y=b_1\\
a_{21}x+a_{22}y=b_2\\
\end{cases}
\end{align} 

1.  The lines intersect at only one point. Then the system has a **unique solution** corresponding to that point.

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

## Consistent and inconsistent linear systems

A system of equations is called **inconsistent** when there is no solution for this system of equations, and it is called **consistent** when there is at least one solution for it.

The graph of $ax+by+cz = d$ (it has three variables) is a plane.

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