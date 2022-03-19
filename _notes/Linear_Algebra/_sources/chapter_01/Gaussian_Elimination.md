# Gaussian Elimination

## Elementary Operations


**Equivalent Matrices**: We say that the matrix $B$ is equivalent to the matrix $A$ provided that $B$ can be obtained from $A$ by performing a sequence of elementary row operations beginning with $A$.


<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem:
</b></font>
    
<ul>
<li><p>The two linear systems of equations corresponding to two equivalent augmented matrices have exactly the same solutions.</p></li>
<li><p>Every matrix <span class="math inline">\(A\)</span> is equivalent to a unique matrix in RREF.</p></li>
</ul>
</div>

<div class="alert alert-block alert-success">
<font size="+1"><b>
Gaussian Algorithm
</b></font>
    
<p><strong>Step 1</strong>: If the matrix consists entirely of zeros, stop—it is already in row-echelon form.</p>
<p><strong>Step 2</strong>: Otherwise, find the first column from the left containing a nonzero entry (call it a ), and move the row containing that entry to the top position.</p>
<p><strong>Step 3</strong>: Now multiply the new top row by 1/a to create a leading 1 .</p>
<p><strong>Step 4</strong>: By subtracting multiples of that row from rows below it, make each entry below the leading 1 zero. This completes the first row, and all further row operations are carried out on the remaining rows.</p>
<p><strong>Step 5</strong>: Repeat steps 1-4 on the matrix consisting of the remaining rows. The process stops when either no rows remain at step 5 or the remaining rows consist entirely of zeros.</p>
</div>


**Back-Substitution**: 
The process of solving a linear system of equations that has been transformed into row-echelon form or reduced row-echelon form. The last equation is solved first, then the next-to-last, etc.

<font color='Blue'><b>Example</b></font>: Solve the following linear system using back-substitution.
\begin{equation*}
\begin{cases}
x_{1}+2\,x_{2}+3\,x_{3}=2\\
4\,x_{1}-3\,x_{2}+x_{3}=-3\\
x_{2}-2\,x_{1}+3\,x_{3}=5
\end{cases}
\end{equation*}

<font color='Green'><b>Solution</b></font>: The corresponding augmented matrix is

$$\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 4 & -3 & 1 & -3\\ -2 & 1 & 3 & 5 \end{array}\right].$$
Use the first row to make the first entry of the second row and third
row zero. That is

\begin{align*}
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ {4} & -3 & 1 & -3\\ -2 & 1 & 3 & 5 \end{array}\right]
&\Rightarrow{-4 R_{1} +R_{2} \rightarrow R_{2}}\Rightarrow
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & -11 & -11 & -11\\ -2 & 1 & 3 & 5 \end{array}\right]\end{align*}

and

\begin{align*}
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & -11 & -11 & -11\\ {-2} & 1 & 3 & 5 \end{array}\right]
&\Rightarrow{2 R_{1} +R_{3} \rightarrow R_{3}}\Rightarrow
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & -11 & -11 & -11\\ 0 & 5 & 9 & 9 \end{array}\right]\end{align*}

Multiply the second row by -1/11 to create a leading 1. We have

\begin{align*}
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & {-11} & -11 & -11\\ 0 & 5 & 9 & 9 \end{array}\right]
&\Rightarrow{-\frac{1}{11}R_{2} \rightarrow R_{2}}\Rightarrow
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & 1 & 1 & 1\\ 0 & 5 & 9 & 9 \end{array}\right]\end{align*}

By subtracting 5 times of the second row from the third row, make entry
below the leading 1 zero.

\begin{align*}
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & 1 & 1 & 1\\ 0 & {5} & 9 & 9 \end{array}\right]
&\Rightarrow{-5 R_{2} +R_{3} \rightarrow R_{3}}\Rightarrow
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & 1 & 1 & 1\\ 0 & 0 & 4 & 4 \end{array}\right]\end{align*}

Finally, we can multiply the last row by 1/4 to create a leading 1. That
is

\begin{align*}
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & 1 & 1 & 1\\ 0 & 0 & {4} & 4 \end{array}\right]
&\Rightarrow{\frac{1}{4}R_{3} \rightarrow R_{3}}\Rightarrow
\left[\begin{array}{ccc|c} {1} & 2 & 3 & 2\\ 0 & {1} & 1 & 1\\ 0 & 0 & {1} & 1 \end{array}\right]\end{align*}
This REF augmented matrix is equivalent to the following linear system:

$$\begin{cases}
x_{1}+2\,x_{2}+3\,x_{3}=2,\\ x_{2}+x_{3}=1,\\ x_{3}=1.
\end{cases}$$

Therefore, $x_{1}=-1$, $x_{2}=0$ and $x_{3}=1$.
***

**homogeneous systems**: A system of equations with the variables $x_1$, $x_2$, ..., $x_n$ is
called **homogeneous** if all the constant terms (RHS) are zero. That
is, if each equation of the system has the form

\begin{equation*}
a_1 x_1 +a_2 x_2 +\ldots+a_n x_n = 0
\end{equation*}

Clearly, $x_1=0$, $x_2=0$, ..., $x_n=0$ is a solution to such a system;
it is called the **trivial solution**. Any solution in which at least
one variable has a nonzero value is called a **nontrivial solution**.

**Example:** The linear system
$\begin{cases}x_{1}+2\,x_{2}=0\\ x_{1}-x_{2}=0\end{cases}$ is
homogeneous. Clearly, $x_1 = 0$ and $x_2 = 0$ is a solution to such a
system; it is called the **trivial solution**. Any solution in which at
least one variable has a nonzero value is called a **nontrivial
solution**.

***

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
free variables in the following linear system $$\begin{cases}
x_{1}-2\,x_{2}-x_{3}=1\\ 2\,x_{1}-4\,x_{2}+x_{3}=5\\ x_{1}-2\,x_{2}+2\,x_{3}=4
\end{cases}$$

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

We can also identify the type of solution from the reduced row-echelon
form of the augmented matrix.

-   **No Solution**: In the case where the system of equations has no
    solution, the row-echelon form of the augmented matrix will have a
    row of the form \begin{align*}
     \left[ \begin{array}{ccc|r}0 & 0 & 0 & 1\\\end{array} \right]. \end{align*}
    This row indicates that the system is inconsistent and has no
    solution.

-   **One Solution**: In the case where the system of equations has one
    solution, every column of the coefficient matrixis apivotcolumn. The
    following is an example of an augmented matrix in reduced
    row-echelon form for a system of equations with one solution.
    
    \begin{align*}
     \left[ \begin{array}{ccc|r}1 & 0 & 0 & 1\\ 0 & 1 & 0 & 2\\ 0 & 0 & 1 & 4\\  \end{array} \right].\end{align*}

-   **Infinitely Many Solutions**: In the case where the system of
    equations has infinitely many solutions, the solution contains
    parameters. There will be columns of the coefficient matrix which
    are not pivot columns. The following are examples of augmented
    matrices in reduced row-echelon form for systems of equations with
    infinitely many solutions.
    
    \begin{align*}
    \left[ \begin{array}{ccc|r}1 & 0 & 0 & 1\\ 0 & 1 & 0 & 2\\ 0 & 0 & 0 & 0\\  \end{array} \right]
    ~\text{ or }
    \left[ \begin{array}{ccc|r}1 & 0 & 0 & 1\\ 0 & 1 & 0 & 2\\  \end{array} \right].\end{align*}

**Example:** Find $h$ so that

$$\left[ \begin{array}{cc|r} 2 &h& 4\\ 3 & 6 & 7\\ \end{array} \right]$$

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

$$6-\frac{3}{2}h=0 \quad \Rightarrow \quad  6=\frac{3}{2}h \quad \Rightarrow \quad 12= 3h \quad \Rightarrow \quad h=4.$$

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***