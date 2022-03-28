# 1.2.3 Homogeneous Equations


<div class="alert alert-info" role="alert">
<font size="+1"><b>
Homogeneous Systems
</b></font>

A system of equations is called **homogeneous** if all the constant terms (right-hand side terms) are zero. In other words,  for a system of equations with the variables $x_1$, $x_2$, ..., $x_n$, we have

\begin{align*}
\begin{cases}
a_{11}x_1+\ldots+a_{1n}x_{n}=0\\
a_{21}x_1+\ldots+a_{2n}x_{n}=0\\
\vdots \\
a_{m1}x_1+\ldots+a_{mn}x_{n}=0.
\end{cases}
\end{align*} 
</div>

Clearly, $x_1=0$, $x_2=0$, ..., $x_n=0$ is a solution to such a system;
it is called the **trivial solution**. Any solution in which at least
one variable has a nonzero value is called a **nontrivial solution**.

<font color='Blue'><b>Example</b></font>: The linear system 
$\begin{cases}x_{1}+2\,x_{2}=0\\ x_{1}-x_{2}=0\end{cases}$ is
homogeneous. Clearly, $x_1 = 0$ and $x_2 = 0$ is a solution to such a
system; it is called the **trivial solution**. Any solution in which at
least one variable has a nonzero value is called a **nontrivial
solution**.

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
A homogeneous system of linear equations always has a trivial solution (consistent).
</div>

**Basic and free variables**: To solve a linear system, the augmented matrix is carried to a reduced
row-echelon form (RREF), and the variables corresponding to the leading
ones are called **basic variables** (leading variables). Because the
matrix is in reduced form, each basic variables occurs in exactly one
equation, so that equation can be solved to give a formula for the basic
variables in terms of the **free variables** (non-leading variables). It
is customary to label-free variables by new variables $s$, $t$, ...,
called parameters.

<font color='Blue'><b>Example</b></font>: Find the basic and
free variables in the following linear system
\begin{align*}
\begin{cases}
x_{1}-2\,x_{2}-x_{3}=1\\ 2\,x_{1}-4\,x_{2}+x_{3}=5\\ x_{1}-2\,x_{2}+2\,x_{3}=4
\end{cases}
\end{align*} 

<font color='Green'><b>Solution</b></font>: The corresponding augmented matrix is

\begin{align*}
\left[\begin{array}{ccc|c} 1 & -2 & -1 & 1\\ 2 & -4 & 1 & 5\\ 1 & -2 & 2 & 4 \end{array}\right].\end{align*}

It follows from subtracting twice row 1 from row 2 and subtracting row 1
from row 3 that

\begin{align*}
\left[\begin{array}{ccc|c} 1 & -2 & -1 & 1\\ 2 & -4 & 1 & 5\\ 1 & -2 & 2 & 4 \end{array}\right]
&\Rightarrow-R_{1} +R_{3} \rightarrow R_{3}, {-2 R_{1} +R_{2} \rightarrow R_{2}} \Rightarrow
\left[\begin{array}{ccc|c} 1 & -2 & -1 & 1\\ 0 & 0 & 3 & 3\\ 0 & 0 & 3 & 3 \end{array}\right]\end{align*}

We also can subtract row 2 from row 3, and then multiply row 2 by

\begin{align*}
\left[\begin{array}{ccc|c} 1 & -2 & -1 & 1\\ 0 & 0 & 3 & 3\\ 0 & 0 & 3 & 3 \end{array}\right]
&\Rightarrow \frac{1}{3}R_{2} \rightarrow R_{2}, {-R_{2} +R_{3} \rightarrow R_{3}}\Rightarrow
\left[\begin{array}{ccc|c} 1 & -2 & -1 & 1\\ 0 & 0 & 1 & 1\\ 0 & 0 & 0 & 0 \end{array}\right]\end{align*}

This is in row-echelon form, and we take it to reduced form by adding row 2 to row 1.

\begin{align*}
\left[\begin{array}{ccc|c} 1 & -2 & -1 & 1\\ 0 & 0 & 1 & 1\\ 0 & 0 & 0 & 0 \end{array}\right]
&\Rightarrow{R_{1} +R_{2} \rightarrow R_{1}} \Rightarrow
\left[\begin{array}{ccc|c} {1} & -2 & 0 & 2\\ 0 & 0 & {1} & 1\\ 0 & 0 & 0 & 0 \end{array}\right]\end{align*}

We can see that columns 1 and 3 are pivot columns. These columns
correspond to variables $x_{1}$ and $x_{3}$ , making these the basic
variables. Column 2 is not a pivot column, which means that $x_{2}$ is a
free variable. We set $x_2={t}$ where $t$ is an arbitrary real number.
Therefore,

$$\begin{cases}
x_{1}-2\,x_{2}=2\\ x_{3}=1\\ 0=0
\end{cases}$$

Let $x_2={t}$ where $t\in \mathbb{R}$

$$
\begin{cases}
x_{1}=2+2t\\ x_{2}=t\\x_{3}=1.
\end{cases}
,\quad t\in \mathbb{R}.$$
***

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
<p>For any system of linear equations exactly one of the following holds:</p>
<ol type="1">
<li><p>The system has <strong>no solutions</strong> (inconsistent).</p></li>
<li><p>The system has a <strong>unique</strong> solution (consistent).</p></li>
<li><p>The system has <strong>infinitely many</strong> solution (consistent).</p></li>
</ol>
</div>

For a system of equations, we can also identify the type of solution from the reduced row-echelon form of the augmented matrix.

-   **No Solution**: a system of equations has no solution if the reduced row-echelon form (RREF) of its augmented matrix has a row of the form
\begin{align*}
\left[ \begin{array}{ccc|r}0 & 0 & 0 & 1\\\end{array} \right].
\end{align*}
This row indicates that the system is **inconsistent** and has no solution.

-   **One Solution**:  a system of equations has one solution if every column of the reduced row-echelon form (RREF) of its augmented matrix is a pivot column. For example, the following matrix shows an augmented matrix in reduced row-echelon form for a system of equations that has only one solution.
    
\begin{align*}
\left[ \begin{array}{ccc|r}1 & 0 & 0 & 1\\ 0 & 1 & 0 & 2\\ 0 & 0 & 1 & 4\\  \end{array} \right].
\end{align*}

-   **Infinitely Many Solutions**: a system of equations has infinitely many solutions if not all columns of the reduced row-echelon form (RREF) of its augmented matrix is a pivot column. For example, the following matrix shows an augmented matrix in reduced row-echelon form for a system of equations that has only one solution.
    
    \begin{align*}
    \left[ \begin{array}{ccc|r}1 & 0 & 0 & 1\\ 0 & 1 & 0 & 2\\ 0 & 0 & 0 & 0\\  \end{array} \right]
    ~\text{ or }
    \left[ \begin{array}{ccc|r}1 & 0 & 0 & 1\\ 0 & 1 & 0 & 2\\  \end{array} \right].\end{align*}
<font color='Blue'><b>Example</b></font>: Find $h$ so that

\begin{align*}
\left[ \begin{array}{cc|r} 2 &h& 4\\ 3 & 6 & 7\\ \end{array} \right].
\end{align*}
is inconsistent.

<font color='Green'><b>Solution</b></font>:

First off, inconsistent means **no solutions**. Let's start by putting
the augmented matrix into REF.

\begin{align*}
\left[\begin{array}{cc|c}2 & h & 4\\3 & 6 & 7 \end{array}\right]
&\Rightarrow{\frac{1}{2}R_{1}\rightarrow R_{1}} \Rightarrow
\left[\begin{array}{cc|c}1 & \frac{h}{2} & 2\\3 & 6 & 7\end{array}\right]
\\
& \Rightarrow{-3R_{1}+R_{2}\rightarrow R_{2}}\Rightarrow
\left[\begin{array}{cc|c}1 & \frac{h}{2} & 2\\0 & 6-\frac{3}{2}h & 1\end{array}\right]\end{align*}

In the case where the system of equations has no solution, the REF of
the augmented matrix should have a row of the form 
$\left[ \begin{array}{cc|c}
1 & * & *\\
0 & 0 & \text{non-zero}\
\end{array} \right]$.

This means that we need to have
\begin{align*}
6-\frac{3}{2}h=0 \quad \Rightarrow \quad  6=\frac{3}{2}h \quad \Rightarrow \quad 12= 3h \quad \Rightarrow \quad h=4.
\end{align*}

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***