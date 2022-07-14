# Systems Of Equations, Algebraic Procedures

We start this section with an example. Consider the following system
\begin{align*}
\begin{cases}
3x_1 +2x_2 - x_3 + x_4 =-1\\
2x_1 - x_3 +2x_4 = 0\\
3x_1 + x_2 +2x_3 +5x_4 = 2
\end{cases}
\end{align*} 
This system of linear equations has three equations and four variables. We can express this in the form of a matrix (an array of numbers) as follows:

\begin{align*}
\left[\begin{array}{cccc|c} 3 & 2 & -1 & 1 & -1\\ 2 & 0 & -1 & 2 & 0\\ 3 & 1 & 2 & 5 & 2 \end{array}\right]
\end{align*} 

This matrix is called the **augmented matrix** of the system.


<div class="alert alert-info" role="alert">
<font size="+1"><b>
Augmented Matrix of a Linear System
</b></font>

For the following system of equations 
\begin{align*}
\begin{cases}
a_{11}x_1+\ldots+a_{1n}x_{n}=b_1\\
a_{21}x_1+\ldots+a_{2n}x_{n}=b_2\\
\vdots \\
a_{m1}x_1+\ldots+a_{mn}x_{n}=b_m,
\end{cases}
\end{align*} 
the augmented matrix can be expressed as follows
\begin{align*}
\left[\begin{array}{cccc|c}
a_{11} & a_{12} & \dots & a_{1n} & b_{1} \\
a_{21} & a_{22} & \dots & a_{2n} & b_{2} \\
\vdots & \vdots & \ddots & \vdots & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn} & b_{m}\\
\end{array}\right]
\end{align*}
</div>


<font color='Blue'><b>Example</b></font>: Express the following linear system in the augmented matrix form.

<font color='Green'><b>Solution</b></font>:
\begin{align*}
\begin{cases}
x_1 + 2x_2 - 2x_3 + x_4 + x_5 =2\\
2x_1 + x_2 + 3x_3 - x_4 =-1\\
x_2 -4x_3 + 3x_4 + x_5 =1\\
\end{cases}
\end{align*} 

<font color='Green'><b>Solution</b></font>: We have,
\begin{align*}
\left[\begin{array}{ccccc|c}
1 & 2 & -2 & 1 & 1 & 2\\
2 & 1 & 3 & -1 & 0 & -1\\
0 & 1 & -4 & 3 & 1 & 1\\
\end{array}\right]
\end{align*} 

## Elementary Operations

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Elementary Operations
</b></font>

The elementary operations can be performed on systems of linear equations to produce equivalent systems. The operations are available as follows:

1.  Interchange two equations.
1.  Multiply one equation by a nonzero number.
1.  Add a multiple of one equation to a different equation.
</div>


<font color='Blue'><b>Example</b></font>: For the following system of equations \begin{align*}\begin{cases}x+2y =3\\ x-y=0\end{cases}\end{align*}
We can

1.  Interchange two equations: \begin{align*}\begin{cases}x-y=0\\ x+2y =3\end{cases}\end{align*}
1.  Multiply the first equation by 5 (a nonzero number): \begin{align*}\begin{cases}5x-5y=0\\ x+2y =3\end{cases}\end{align*}
1.  Add (-3) times of the second equation to the first equation:
\begin{align*}\begin{cases}5x-5y-3(x+2y)=0-3(3)\\x+2y =3\end{cases}
&\Rightarrow
\begin{cases}5x-3x-5y-6y=0-9\\x+2y =3\end{cases} \\&\Rightarrow
\begin{cases}2x-11y=-9\\x+2y =3\end{cases}
\end{align*}

In hand calculations (and in computer programs), we manipulate the rows of the augmented matrix rather than the equations.

***

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Elementary Row Operations:
</b></font>

Elementary row operations on a matrix:

1.  Interchange two rows.
1.  Multiply one row by a nonzero number.
1.  Add a multiple of one row to a different row.
</div>



<font color='Blue'><b>Example</b></font>: For the system of equations from the previous example, first, we need to write down the system in the
augmented matrix form. We have
\begin{align*}\left[\begin{array}{cc|c} 1 & 2 & 3\\ 1 & -1 & 0 \end{array}\right]\end{align*}

Let $R_{1}$ and $R_{2}$ denote the first row and the second row of the
current augmented matrix, respectively.

1.  Interchange the first and the second row:
\begin{align*}\left[\begin{array}{cc|c} 1 & 2 & 3\\ 1 & -1 & 0 \end{array}\right]
\Rightarrow{R_{1} \leftrightarrow R_{2}}\Rightarrow
\left[\begin{array}{cc|c} 1 & -1 & 0 \\ 1 & 2 & 3\end{array}\right]\end{align*}

1.  Multiply the first row by 5 (a nonzero number):
\begin{align*}\left[\begin{array}{cc|c} 1 & -1 & 0 \\ 1 & 2 & 3\end{array}\right]
\Rightarrow{5 R_{1} \rightarrow R_{1}}\Rightarrow
\left[\begin{array}{cc|c} 5 & -5 & 0 \\ 1 & 2 & 3\end{array}\right]\end{align*}

1.  Add (-3) times of the second row to the first row: \begin{align*}
\left[\begin{array}{cc|c} 5 & -5 & 0 \\ 1 & 2 & 3\end{array}\right]
\Rightarrow{-3 R_{2} +R_{1} \rightarrow R_{1}}\Rightarrow
\left[\begin{array}{cc|c} 2 & -11 & -9 \\ 1 & 2 & 3\end{array}\right]
\end{align*}

<div class="alert alert-warning" role="alert">
<font size="+1"><b>
A compact notation to describe elementary operations:
</b></font>

|           Operation description           |              Notation             |
|:-----------------------------------------:|:---------------------------------:|
|        Interchange rows $i$ and $j$       |   $R_{i} \leftrightarrow R_{j}$   |
| Multiply row $i$ by $s$, where $s \neq 0$ |     $R_{i} \rightarrow R_{i}$     |
|      Add $s$ times row $i$ to row $j$     | $R_{i} + R_{j} \rightarrow R_{j}$ |
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
(Reduced) Row-Echelon Form
</b></font>

A matrix is said to be in **Row-Echelon Form** (REF) if it meets the following three conditions:

1.  All **zero rows** (consisting entirely of zeros) are at the bottom.

1.  The first nonzero entry from the left in each nonzero row is a 1,
    called the **leading 1** for that row.

1.  Each leading 1 is to the right of all leading 1 s in the rows above
    it.
A row-echelon matrix is said to be in **reduced row-echelon form**
(RREF) if, in addition to the above three, it satisfies the following condition:

1.  Each leading 1 is the only nonzero entry in its column.
</div>

<font color='Blue'><b>Example</b></font>: In each case identify whether the augmented matrix is RREF or REF.

a).
\begin{align*}\left[ \begin{array}{cc|c}    2 & 0 & 0 \\     0 & 1 & 1\\     0 & 0 & 2 \\     0 & 0 & 0 \\    \end{array} \right]\end{align*}

-   All zero rows are at the bottom. $\surd$

-   The first nonzero entry from the left in each nonzero row is not
    a 1. ${\color{red}X}$

Therefore it is not REF (If a matrix is not REF, it is not RREF as
well).


b).
\begin{align*}\left[ \begin{array}{ccccc|c}
1 & 3 & 0 & 5 & 0 & -1 \\
0 & 0 & 1 & 1 & 2 & 3 \\
0 & 0 & 0 & 0 & 1 & 2 \\
\end{array} \right]\end{align*}

-   All zero rows are at the bottom (we don't have any all-zero rows
    here). $\surd$

-   The first nonzero entry from the left in each nonzero row is a 1.
    $\surd$

-   Each leading 1 is to the right of all leading 1 s in the rows above
    it. $\surd$

Therefore, it is a REF. However, Each leading 1 is not the only nonzero entry in its column. Therefore, it is not RREF.

## Gaussian Elimination


<div class="alert alert-info" role="alert">
<font size="+1"><b>
Equivalent Matrices
</b></font>

The matrix $B$ is equivalent to the matrix $A$ if $B$ can be produced by a sequence of elementary row operations starting with $A$.
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem:
</b></font>

* Two linear systems have exactly the same solutions if corresponding augmented matrices of two linear systems of equations are equivalent.
* Every matrix is equivalent to a unique matrix in RREF.
</div>

<div class="alert alert-block alert-success">
<font size="+1"><b>
Gaussian Algorithm: For a matrix $A$, 
</b></font>
<p><strong>Step 1</strong>: If the matrix $A$ only consists entirely of zeros, stop. It is already in REF.
<p><strong>Step 2</strong>: Otherwise, identify the first column from the left comprising a nonzero entry (let's call this entry $a$) and move the row containing that entry to the top position.</p>
<p><strong>Step 3</strong>: Now multiply the new top row by $1/a$ to create a leading 1 .</p>
<p><strong>Step 4</strong>: By subtracting multiples of that row from rows underneath it, make each entry below the leading 1 zero. This completes the first row, and all additional row operations are conducted on the rest of the rows.</p>
<p><strong>Step 5</strong>: Repeat steps 1-4 on the matrix consisting of the remaining rows. The process is carried out iteratively until either no rows remain at step 5 or the remaining rows consist entirely of zeros.</p>
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Back-Substitution
</b></font>

Back-substitution is a process of solving a linear system of equations using its REF or RREF. In this process, the last equation is solved first, then the second last equation is solved next, etc.
</div>

<font color='Blue'><b>Example</b></font>: Solve the following linear system using back-substitution.
\begin{align*}
\begin{cases}
x_{1}+2\,x_{2}+3\,x_{3}=2\\
4\,x_{1}-3\,x_{2}+x_{3}=-3\\
x_{2}-2\,x_{1}+3\,x_{3}=5
\end{cases}
\end{align*}

<font color='Green'><b>Solution</b></font>: The corresponding augmented matrix is

\begin{align*}
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 4 & -3 & 1 & -3\\ -2 & 1 & 3 & 5 \end{array}\right].
\end{align*}
Use the first row to make the first entry of the second row and third row zero. That is

\begin{align*}
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ {4} & -3 & 1 & -3\\ -2 & 1 & 3 & 5 \end{array}\right]
&\Rightarrow{-4 R_{1} +R_{2} \rightarrow R_{2}}\Rightarrow
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & -11 & -11 & -11\\ -2 & 1 & 3 & 5 \end{array}\right]
\end{align*}

and

\begin{align*}
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & -11 & -11 & -11\\ {-2} & 1 & 3 & 5 \end{array}\right]
&\Rightarrow{2 R_{1} +R_{3} \rightarrow R_{3}}\Rightarrow
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & -11 & -11 & -11\\ 0 & 5 & 9 & 9 \end{array}\right]
\end{align*}

Multiply the second row by -1/11 to create a leading 1. We have

\begin{align*}
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & {-11} & -11 & -11\\ 0 & 5 & 9 & 9 \end{array}\right]
&\Rightarrow{-\frac{1}{11}R_{2} \rightarrow R_{2}}\Rightarrow
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & 1 & 1 & 1\\ 0 & 5 & 9 & 9 \end{array}\right]
\end{align*}

By subtracting 5 times of the second row from the third row, make entry
below the leading 1 zero.

\begin{align*}
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & 1 & 1 & 1\\ 0 & {5} & 9 & 9 \end{array}\right]
&\Rightarrow{-5 R_{2} +R_{3} \rightarrow R_{3}}\Rightarrow
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & 1 & 1 & 1\\ 0 & 0 & 4 & 4 \end{array}\right]
\end{align*}

Finally, we can multiply the last row by 1/4 to create a leading 1. That
is

\begin{align*}
\left[\begin{array}{ccc|c} 1 & 2 & 3 & 2\\ 0 & 1 & 1 & 1\\ 0 & 0 & {4} & 4 \end{array}\right]
&\Rightarrow{\frac{1}{4}R_{3} \rightarrow R_{3}}\Rightarrow
\left[\begin{array}{ccc|c} {1} & 2 & 3 & 2\\ 0 & {1} & 1 & 1\\ 0 & 0 & {1} & 1 \end{array}\right]
\end{align*}
This REF augmented matrix is equivalent to the following linear system:

\begin{align*}
\begin{cases}
x_{1}+2\,x_{2}+3\,x_{3}=2,\\ x_{2}+x_{3}=1,\\ x_{3}=1.
\end{cases}
\end{align*}

Therefore, $x_{1}=-1$, $x_{2}=0$ and $x_{3}=1$.


## Homogeneous Equations


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

Clearly, $x_1=0$, $x_2=0$, ..., $x_n=0$ is a solution to such a system which is also known as the **trivial solution**. Note that any solution that has a nonzero component is called a  **nontrivial solution**.

<font color='Blue'><b>Example</b></font>: The linear system $\begin{cases}x_{1}+2\,x_{2}=0\\ x_{1}-x_{2}=0\end{cases}$ is homogeneous. Clearly, $x_1 = 0$ and $x_2 = 0$ is a solution to such a system; it is called the **trivial solution**. Any solution in which at least one variable has a nonzero value is called a **nontrivial
solution**.

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
A homogeneous system of linear equations always has a trivial solution (consistent).
</div>

Solving a linear system using an augmented matrix requires a reduced
row-echelon form (RREF). In this form, the variables corresponding to
the leading ones are called <strong>basic variables</strong> (leading
variables) and each basic variable emerges in exactly one equation
(because the matrix is in reduced form). Therefore, each equation can be
solved to provide a formula for the basic variables in terms of the
<strong>free variables</strong> (non-leading variables). It is standard
to label these free variables by new variables <span
class="math inline">\(s$, <span
class="math inline">\(t$, …, called parameters.

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


## Rank of a matrix

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Rank of a Matrix
</b></font>

The rank of matrix $A$ is the number of leading 1s in the reduced row-echelon form (RREF) of the matrix $A$.
</div>


<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem:
</b></font>
    
Consider following system of equations with $m$ equations in $n$ variables
\begin{align*}
\begin{cases}
a_{11}x_1+\ldots+a_{1n}x_{n}=0\\
a_{21}x_1+\ldots+a_{2n}x_{n}=0\\
\vdots \\
a_{m1}x_1+\ldots+a_{mn}x_{n}=0.
\end{cases}
\end{align*} 
Suppose that the rank of the augmented matrix is $r$. Then

* If $r<n$ , the system has **infinitely many solutions**.
* If $r = n$ , the system has **a unique solution**.
</div>


<font color='Blue'><b>Example</b></font>: Consider the following system of equations 

$$
\begin{cases}
x_{1}-2\,x_{2}-x_{3}=1\\ 2\,x_{1}-4\,x_{2}+x_{3}=5\\ x_{1}-2\,x_{2}+2\,x_{3}=4
\end{cases}
$$

<font color='Green'><b>Solution</b></font>: The corresponding augmented matrix is

\begin{align*}
\left[\begin{array}{ccc|c} 1 & -2 & -1 & 1\\ 2 & -4 & 1 & 5\\ 1 & -2 & 2 & 4 \end{array}\right].\end{align*}

From previous examples, we know the RREF of this matrix is

\begin{align*}
\left[\begin{array}{ccc|c} {1} & -2 & 0 & 2\\ 0 & 0 & {1} & 1\\ 0 & 0 & 0 & 0 \end{array}\right]\end{align*}

It can be seen that $r=Rank(A)=2$ and the number of variables is $n=3$.
From the above theorem, we know that if $r < n$ , the system has
**infinitely many solutions**.
***

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Linear Combinations
</b></font>

Let $X_1,~X_2,~\ldots,~X_n$, $V$ be column matrices (each of them consists of only one column). Then, $V$ is said to be a **linear combination** of the columns $X_1,~X_2,~\ldots,~X_n$ if there exist scalars, $a_1,~a_2,~\ldots,~a_n$ such that

\begin{align*}
V=a_1X_1+a_2X_2+\ldots+a_nX_n.
\end{align*}

In other words, $V$ is a **linear combination** of the columns $X_1,~X_2,~\ldots,~X_n$ if it can be expressed in terms of those column matrices.
</div>

<font color='Blue'><b>Example</b></font>:
Let $X_1=\begin{bmatrix} 1 \\ 2 \\ 3\end{bmatrix}$ and
$X_2=\begin{bmatrix} 2 \\ 1 \\ 1\end{bmatrix}$. Then

\begin{align*}
V&=2\begin{bmatrix} 1 \\ 2 \\ 3\end{bmatrix}+3\begin{bmatrix} 2 \\ 1 \\ 1\end{bmatrix}
\\ &
=\begin{bmatrix} (2)(1) \\ (2)(2) \\ (2)(3)\end{bmatrix}+3\begin{bmatrix} (3)(2) \\ (3)(1) \\ (3)(1)\end{bmatrix}
\\ &
=\begin{bmatrix} 2\\ 4\\ 6\end{bmatrix}+3\begin{bmatrix} 6\\ 3\\ 3\end{bmatrix}
=\begin{bmatrix}8\\ 7\\ 9\end{bmatrix}\end{align*}

is a linear
combination of $X_1$ and $X_2$.
***

<font color='Blue'><b>Example</b></font>:
Find all values of $r$ so that $V=\begin{bmatrix}1\\r\\0\end{bmatrix}$
is a linear combination of $X_1=\begin{bmatrix}2\\-1\\1\end{bmatrix}$
and $X_2=\begin{bmatrix}3\\3\\2\end{bmatrix}$.

<font color='Green'><b>Solution</b></font>:
Since $V$ is a linear combinations of $X_1$ and $X_2$, there exist $a$
and $b$ such that

\begin{align*}
V&=aX_1+bX_2,
\\
\begin{bmatrix}1\\r\\0\end{bmatrix}&=a\begin{bmatrix}2\\-1\\1\end{bmatrix}+b\begin{bmatrix}3\\3\\2\end{bmatrix},
\\
\begin{bmatrix}1\\r\\0\end{bmatrix}&=\begin{bmatrix}2a\\-a\\a\end{bmatrix}+\begin{bmatrix}3b\\3b\\2b\end{bmatrix}\end{align*}

However, the last equation is equivalent to

$$\begin{cases}
2a+3b=1\\
-a+3b=r\\
a+2b=0.
\end{cases}$$

The corresponding augmented matrix is

$$\label{Ex1.16.eq.01}
\left[\begin{array}{cc|c} 2 & 3 & 1\\ -1 & 3 & r\\ 1 & 2 & 0 \end{array}\right]$$

REF:

\begin{align*}
\left[\begin{array}{cc|c} 2 & 3 & 1\\ -1 & 3 & r\\ 1 & 2 & 0 \end{array}\right]
&\Rightarrow{R_{1} \leftrightarrow R_{3}} \Rightarrow
\left[\begin{array}{cc|c} 1 & 2 & 0\\ -1 & 3 & r\\ 2 & 3 & 1 \end{array}\right]
\\ &
\Rightarrow -2R_{1}+R_{3}\rightarrow R_{3}, {R_{1}+R_{2}\rightarrow R_{2}} \Rightarrow
\left[\begin{array}{cc|c} 1 & 2 & 0\\ 0 & 5 & r\\ 0 & -1 & 1 \end{array}\right]
\\ &
\Rightarrow{R_{2} \leftrightarrow R_{3}} \Rightarrow
\left[\begin{array}{cc|c} 1 & 2 & 0\\ 0 & -1 & 1\\ 0 & 5 & r \end{array}\right]
\\ &
\Rightarrow{-R_{2}\rightarrow R_{2}} \Rightarrow
\left[\begin{array}{cc|c} 1 & 2 & 0\\ 0 & 1 & -1\\ 0 & 5 & r \end{array}\right]
\\ &
\Rightarrow{-5R_{2}+R_{3}\rightarrow R_{3}} \Rightarrow
\left[\begin{array}{cc|c} {1} & 2 & 0\\ 0 & {1} & -1\\ 0 & 0 & r+5 \end{array}\right]\end{align*}

Note that the linear system is inconsistent if $r+5\neq 0$, and the linear system is consistent
if $r+5= 0$. Therefore, since we are looking for a solution for this
system, only  $r = -5$ is acceptable.

***
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***