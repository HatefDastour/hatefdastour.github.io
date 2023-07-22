# Systems Of Equations, Algebraic Procedures

Let's begin this section with an example. Consider the following system of linear equations:

\begin{align}
\begin{cases}
3x_1 + 2x_2 - x_3 + x_4 &= -1 \\
2x_1 - x_3 + 2x_4 &= 0 \\
3x_1 + x_2 + 2x_3 + 5x_4 &= 2
\end{cases}
\end{align}

This system consists of three equations and four variables. We can represent this system using a matrix (an array of numbers) in the following way:

\begin{align}
\left[\begin{array}{cccc|c}
3 & 2 & -1 & 1 & -1 \\
2 & 0 & -1 & 2 & 0 \\
3 & 1 & 2 & 5 & 2
\end{array}\right]
\end{align}

This matrix is known as the **augmented matrix** of the system.

The augmented matrix is a convenient representation of a system of linear equations. It combines the coefficients and constants of the equations into a single matrix, making it easier to perform various operations and transformations when solving the system. The vertical bar separates the coefficient matrix (the left part) from the constants matrix (the right part). Augmented matrices play a crucial role in techniques like Gaussian elimination and matrix row operations, which are used to find solutions to systems of linear equations.


`````{admonition} Augmented Matrix of a Linear System
:class: tip

For the following system of equations 
\begin{align}
\begin{cases}
a_{11}x_1+\ldots+a_{1n}x_{n}=b_1\\
a_{21}x_1+\ldots+a_{2n}x_{n}=b_2\\
\vdots \\
a_{m1}x_1+\ldots+a_{mn}x_{n}=b_m,
\end{cases}
\end{align} 
the augmented matrix can be expressed as follows
\begin{align}
\left[\begin{array}{cccc|c}
a_{11} & a_{12} & \dots & a_{1n} & b_{1} \\
a_{21} & a_{22} & \dots & a_{2n} & b_{2} \\
\vdots & \vdots & \ddots & \vdots & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn} & b_{m}\\
\end{array}\right]
\end{align}

`````

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


`````{admonition} Elementary Operations
:class: tip

Elementary operations can be applied to systems of linear equations, resulting in equivalent systems. These operations are as follows:

1. **Interchange two equations**: This operation involves swapping the positions of two equations in the system. The resulting system remains equivalent to the original one.

2. **Multiply one equation by a nonzero number**: This operation entails multiplying all terms of an equation by a nonzero constant. The new system obtained is equivalent to the initial system.

3. **Add a multiple of one equation to a different equation**: In this operation, a multiple of one equation is added to another equation in the system. As a result, the new system remains equivalent to the original system.

`````

Elementary operations are fundamental in solving systems of linear equations through techniques like Gaussian elimination and matrix row operations. By performing these operations, we can manipulate the equations to simplify the system and eventually determine its solutions. The goal is to transform the system into a more manageable form, such as row echelon form or reduced row echelon form, which reveals the solutions of the system.

<font color='Blue'><b>Example</b></font>: Consider the following system of equations:

\begin{align*}
\begin{cases}
x + 2y &= 3 \\
x - y &= 0
\end{cases}
\end{align*}

We can perform the following operations:

1. **Interchange two equations**:
\begin{align*}
\begin{cases}
x - y &= 0 \\
x + 2y &= 3
\end{cases}
\end{align*}

2. **Multiply the first equation by 5 (a nonzero number)**:
\begin{align*}
\begin{cases}
5x - 5y &= 0 \\
x + 2y &= 3
\end{cases}
\end{align*}

3. **Add (-3) times the second equation to the first equation**:
\begin{align*}\begin{cases}5x-5y-3(x+2y)=0-3(3)\\x+2y =3\end{cases}
&\Rightarrow
\begin{cases}5x-3x-5y-6y=0-9\\x+2y =3\end{cases} \\&\Rightarrow
\begin{cases}2x-11y=-9\\x+2y =3\end{cases}
\end{align*}

In hand calculations (and in computer programs), we manipulate the rows of the augmented matrix instead of the equations. This process involves applying elementary row operations to the augmented matrix, as shown in the example above, to simplify the system of equations and reveal its solutions.

***

`````{admonition} Elementary Row Operations:
:class: tip

Elementary row operations on a matrix:

1.  Interchange two rows.
1.  Multiply one row by a nonzero number.
1.  Add a multiple of one row to a different row.


`````



<font color='Blue'><b>Example</b></font>: To work with the system of equations from the previous example, we first express it in augmented matrix form:

\begin{align*}
\left[\begin{array}{cc|c}
1 & 2 & 3 \\
1 & -1 & 0
\end{array}\right]
\end{align*}

Let $R_{1}$ and $R_{2}$ denote the first row and the second row of the current augmented matrix, respectively.

1. **Interchange the first and the second row**:
\begin{align*}
\left[\begin{array}{cc|c}
1 & 2 & 3 \\
1 & -1 & 0
\end{array}\right]
\Rightarrow {R_{1} \leftrightarrow R_{2}} \Rightarrow
\left[\begin{array}{cc|c}
1 & -1 & 0 \\
1 & 2 & 3
\end{array}\right]
\end{align*}

2. **Multiply the first row by 5 (a nonzero number)**:
\begin{align*}
\left[\begin{array}{cc|c}
1 & -1 & 0 \\
1 & 2 & 3
\end{array}\right]
\Rightarrow {5 R_{1} \rightarrow R_{1}} \Rightarrow
\left[\begin{array}{cc|c}
5 & -5 & 0 \\
1 & 2 & 3
\end{array}\right]
\end{align*}

3. **Add (-3) times the second row to the first row**:

\begin{align*}
\left[\begin{array}{cc|c}
5 & -5 & 0 \\
1 & 2 & 3
\end{array}\right]
\Rightarrow {-3 R_{2} + R_{1} \rightarrow R_{1}} \Rightarrow
\left[\begin{array}{cc|c}
2 & -11 & -9 \\
1 & 2 & 3
\end{array}\right]
\end{align*}

By performing these elementary row operations on the augmented matrix, we can simplify the system of equations and find its solutions more efficiently.

`````{admonition} Remark: A compact notation to describe elementary operations:
:class: tip



|           Operation description           |              Notation             |
|:-----------------------------------------:|:---------------------------------:|
|        Interchange rows $i$ and $j$       |   $R_{i} \leftrightarrow R_{j}$   |
| Multiply row $i$ by $s$, where $s \neq 0$ |     $R_{i} \rightarrow R_{i}$     |
|      Add $s$ times row $i$ to row $j$     | $R_{i} + R_{j} \rightarrow R_{j}$ |


`````

`````{admonition} (Reduced) Row-Echelon Form
:class: tip

A matrix is considered to be in **Row-Echelon Form** (REF) if it satisfies the following three conditions:

1. All **zero rows** (rows consisting entirely of zeros) are placed at the bottom of the matrix.

1. The first nonzero entry from the left in each nonzero row is equal to 1, and it is referred to as the **leading 1** for that specific row.

1. Each leading 1 is positioned to the right of all leading 1s present in the rows above it.

A row-echelon matrix is classified as being in **Reduced Row-Echelon Form** (RREF) if, in addition to the aforementioned three conditions, it also fulfills the following condition:

1. Each leading 1 is the only nonzero entry in its respective column.


`````

The Row-Echelon Form and Reduced Row-Echelon Form of a matrix are significant concepts in linear algebra. These forms are attained through a series of elementary row operations, such as row swaps, row scaling, and row replacements, which simplify the matrix and bring it into a more structured and easily solvable format. These forms are crucial in solving systems of linear equations and performing various operations on matrices.

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


`````{admonition} Equivalent Matrices
:class: tip

The matrix $B$ is equivalent to the matrix $A$ if $B$ can be produced by a sequence of elementary row operations starting with $A$.

`````

```{admonition} Theorem

* Two linear systems have exactly the same solutions if corresponding augmented matrices of two linear systems of equations are equivalent.
* Every matrix is equivalent to a unique matrix in RREF.
```

`````{admonition} Gaussian Algorithm: For a matrix $A$, 
:class: caution

**Step 1**: If the matrix A only consists entirely of zeros, stop. It is already in REF.

**Step 2**: Otherwise, identify the first column from the left comprising a nonzero entry (let's call this entry a) and move the row containing that entry to the top position.

**Step 3**: Now multiply the new top row by 1/a to create a leading 1.

**Step 4**: By subtracting multiples of that row from rows underneath it, make each entry below the leading 1 zero. This completes the first row, and all additional row operations are conducted on the rest of the rows.

**Step 5**: Repeat steps 1-4 on the matrix consisting of the remaining rows. The process is carried out iteratively until either no rows remain at step 5 or the remaining rows consist entirely of zeros.

`````

`````{admonition} Back-Substitution
:class: tip

Back-substitution is a method used to solve a linear system of equations by utilizing its Row-Echelon Form (REF) or Reduced Row-Echelon Form (RREF). In this process, we start by solving the last equation in the REF/RREF, then move on to solving the second-to-last equation, and so on.

`````

By working backward from the last equation to the first, we can efficiently find the values of the variables in the system. This approach takes advantage of the simplified structure of the REF/RREF, where each equation typically involves only one variable, making it easier to isolate and determine the values of the variables step by step.

Back-substitution is a powerful technique used in numerical methods and linear algebra, particularly in solving systems of linear equations with large matrices. It is commonly employed in algorithms and computer programs for efficient and accurate solutions.

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


`````{admonition} Homogeneous Systems
:class: tip

A system of equations is referred to as **homogeneous** if all the constant terms (right-hand side terms) are zero. In other words, for a system of equations with the variables $x_1$, $x_2$, $\ldots$, $x_n$, we have:

\begin{align}
\begin{cases}
a_{11}x_1 + \ldots + a_{1n}x_{n} &= 0 \\
a_{21}x_1 + \ldots + a_{2n}x_{n} &= 0 \\
\vdots \\
a_{m1}x_1 + \ldots + a_{mn}x_{n} &= 0.
\end{cases}
\end{align}

`````

In a homogeneous system, all the equations represent linear combinations of the variables that sum to zero. This means that if we substitute the values of the variables into each equation, the left-hand side of each equation will always equal zero.

Homogeneous systems are of particular interest in linear algebra, as they have nontrivial solutions (solutions where not all variables are equal to zero) apart from the trivial solution (all variables equal to zero). These nontrivial solutions play a critical role in various applications, such as understanding the null space of a matrix, eigenvectors and eigenvalues, and the properties of linear transformations.


`````{admonition} Remark
:class: important

Undoubtedly, the solution $x_1=0$, $x_2=0$, ..., $x_n=0$ is a valid solution to such a system, and it is commonly referred to as the **trivial solution**. In the trivial solution, all variables $x_1, x_2, \ldots, x_n$ are set to zero.

However, any solution that contains at least one nonzero component is known as a **nontrivial solution**. In a nontrivial solution, at least one variable has a value other than zero, resulting in a non-zero combination when substituted into the system of equations. These nontrivial solutions are particularly noteworthy as they provide insight into the diverse possibilities of solutions for a homogeneous system of equations.

`````

It is important to distinguish between the trivial and nontrivial solutions, as the presence of nontrivial solutions indicates that the homogeneous system has alternative solutions beyond the obvious all-zero solution. These nontrivial solutions hold significant importance in various mathematical applications and analyses.


<font color='Blue'><b>Example</b></font>: The linear system $\begin{cases}x_{1}+2\,x_{2}=0\\ x_{1}-x_{2}=0\end{cases}$ is homogeneous. Clearly, $x_1 = 0$ and $x_2 = 0$ is a solution to such a system; it is called the **trivial solution**. Any solution in which at least one variable has a nonzero value is called a **nontrivial
solution**.

`````{admonition} Remark
:class: important

Every homogeneous system of linear equations is guaranteed to possess a **trivial solution** (consistent solution) where all the variables are set to zero. This solution results in all equations being satisfied simultaneously when the variables are substituted with zero.

In a homogeneous system, this trivial solution is distinct from other **nontrivial solutions**, which involve at least one variable having a nonzero value. Nontrivial solutions arise when the system has infinitely many solutions due to the presence of free variables or when it has no solutions at all. However, the existence of the trivial solution is constant for any homogeneous system, and it plays a fundamental role in linear algebra, especially when investigating the properties of null spaces and linear transformations.

`````

To solve a linear system using an augmented matrix, it is necessary to convert the matrix into its Reduced Row-Echelon Form (RREF). In this form, the variables associated with the leading ones are referred to as **basic variables** or **leading variables** since they dictate the system's structure and are the foundation for finding solutions. Each basic variable appears in exactly one equation because the matrix is in reduced form.

By expressing each equation in terms of the basic variables, it is possible to derive formulas for these variables solely based on the values of the **free variables** (also known as non-leading variables). In linear algebra, it is customary to denote these free variables as new variables such as $s$, $t$, etc., and they are often referred to as **parameters**.

Solving systems in RREF form and using parameters for the free variables simplifies the process of finding solutions. The parameterization allows us to express the solutions in a more compact and general form, making it easier to analyze the behavior of the system across different parameter values. This approach is a standard technique in linear algebra, particularly in understanding the geometric and algebraic properties of linear systems and their solutions.


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

We can see that columns 1 and 3 are pivot columns. These columns correspond to variables $x_{1}$ and $x_{3}$ , making these the basic variables. Column 2 is not a pivot column, which means that $x_{2}$ is a
free variable. We set $x_2={t}$ where $t$ is an arbitrary real number. Therefore,

\begin{align*}
\begin{cases}
x_{1}-2\,x_{2}=2\\ x_{3}=1\\ 0=0
\end{cases}
\end{align*}

Let $x_2={t}$ where $t\in \mathbb{R}$

\begin{align*}
\begin{cases}
x_{1}=2+2t\\ x_{2}=t\\x_{3}=1.
\end{cases}
,\quad t\in \mathbb{R}.
\end{align*}
***

`````{admonition} Remark
:class: important
For any system of linear equations, one and only one of the following possibilities is true:

1. The system has **no solutions** (inconsistent), meaning there is no set of values for the variables that satisfy all the equations simultaneously. In this case, the system represents a set of contradictory or parallel lines in the geometric interpretation.

2. The system has a **unique solution** (consistent), indicating that there is precisely one set of values for the variables that satisfy all the equations. Geometrically, this corresponds to the intersection of the lines representing the equations at a single point.

3. The system has **infinitely many solutions** (consistent), signifying that there are multiple sets of values for the variables that satisfy all the equations. In the geometric interpretation, this represents a situation where the equations' lines overlap or coincide, resulting in an infinite number of intersection points.

`````

These three possibilities encompass all potential outcomes for a system of linear equations. The nature of the solution is essential in understanding the behavior of the system and is determined based on the coefficients and constants in the equations. Solving linear systems involves identifying which of these three scenarios holds true and finding the solutions accordingly.

For a system of equations, the type of solution can also be determined from the Reduced Row-Echelon Form (RREF) of its augmented matrix. Let's explore each possibility:

- **No Solution**: A system of equations has no solution if the RREF of its augmented matrix contains a row of the form:

\begin{align*}
\left[ \begin{array}{ccc|r}
0 & 0 & 0 & 1 \\
\end{array} \right].
\end{align*}

This row indicates that the system is **inconsistent**, and it does not have a solution. Geometrically, this means that the equations represent parallel lines that do not intersect.

- **One Solution**: A system of equations has one solution if every column of the RREF of its augmented matrix is a pivot column. The RREF of the augmented matrix for a system with one solution appears as follows:

\begin{align*}
\left[ \begin{array}{ccc|r}
1 & 0 & 0 & 1 \\
0 & 1 & 0 & 2 \\
0 & 0 & 1 & 4 \\
\end{array} \right].
\end{align*}

In this case, the system is **consistent**, and it has a unique solution. Geometrically, this corresponds to the intersection of the equations' lines at a single point.

- **Infinitely Many Solutions**: A system of equations has infinitely many solutions if not all columns of the RREF of its augmented matrix are pivot columns. The RREF of the augmented matrix for a system with infinitely many solutions is shown below:

\begin{align*}
\left[ \begin{array}{ccc|r}
1 & 0 & 2 & 3 \\
0 & 1 & -1 & 1 \\
0 & 0 & 0 & 0 \\
\end{array} \right].
\end{align*}

In this scenario, the system is **consistent**, and it has multiple solutions. Geometrically, this represents overlapping or coinciding lines, resulting in an infinite number of intersection points.

By examining the RREF of the augmented matrix, we can determine the nature of the solution for the corresponding system of equations. The RREF serves as a crucial tool in solving linear systems and understanding their solution behavior.
    
\begin{align*}
\left[ \begin{array}{ccc|r}1 & 0 & 0 & 1\\ 0 & 1 & 0 & 2\\ 0 & 0 & 0 & 0\\  \end{array} \right]
~\text{ or }
\left[ \begin{array}{ccc|r}1 & 0 & 0 & 1\\ 0 & 1 & 0 & 2\\  \end{array} \right].
\end{align*}

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

`````{admonition} Definition
:class: tip
Rank of a Matrix

The **rank** of a matrix $A$ is defined as the number of leading 1s in its Reduced Row-Echelon Form (RREF). When we perform Gaussian elimination or use other row-reduction techniques to convert the matrix $A$ into its RREF, we can count the number of leading 1s to determine its rank.

`````

The rank of a matrix is a fundamental concept in linear algebra, and it has various important implications in the study of systems of linear equations, linear transformations, and the properties of matrices. The rank reflects the dimension of the column space (also known as the image or range) and the row space of the matrix, which in turn provides insight into the linear independence and the existence of solutions to systems of equations.

Additionally, the rank of a matrix is related to the dimension of its null space (kernel) and is used to characterize the properties of invertibility and determinant in square matrices. Understanding the rank is crucial in many practical applications, such as solving linear systems, image and signal processing, data analysis, and machine learning.

```{admonition} Theorem
Theorem:
    
Consider the following system of equations with $m$ equations in $n$ variables:

\begin{align*}
\begin{cases}
a_{11}x_1 + \ldots + a_{1n}x_{n} = 0 \\
a_{21}x_1 + \ldots + a_{2n}x_{n} = 0 \\
\vdots \\
a_{m1}x_1 + \ldots + a_{mn}x_{n} = 0.
\end{cases}
\end{align*}
Suppose that the rank of the augmented matrix is $r$. Then:

- If $r < n$, the system has **infinitely many solutions**. In this case, there are more variables ($n$) than there are linearly independent equations, which means that the system contains free variables. The presence of free variables leads to an infinite number of solutions, where each solution is parameterized by the values of the free variables. Geometrically, this corresponds to a situation where the equations represent overlapping or coinciding planes or lines, resulting in infinite intersection points.

- If $r = n$, the system has **a unique solution**. When the rank of the augmented matrix is equal to the number of variables ($n$), the system of equations contains exactly enough linearly independent equations to determine a unique solution for each variable. Geometrically, this corresponds to the equations representing $n$ non-parallel planes (in 3D) or $n$ non-collinear lines (in 2D) that intersect at a single point, leading to a unique solution for the system.


```

The rank of the augmented matrix is a critical factor in determining the nature of the solutions to the system of linear equations. It reveals important information about the linear independence of the equations and the existence of solutions, providing valuable insights into the properties and behavior of the system.

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

`````{admonition} Linear Combinations
:class: tip

Let $X_1,~X_2,~\ldots,~X_n$ and $V$ be column matrices (each consisting of only one column). We say that $V$ is a **linear combination** of the columns $X_1,~X_2,~\ldots,~X_n$ if there exist scalars $a_1,~a_2,~\ldots,~a_n$ such that:

\[
V = a_1X_1 + a_2X_2 + \ldots + a_nX_n.
\]

In simpler terms, $V$ is a **linear combination** of the columns $X_1,~X_2,~\ldots,~X_n$ if it can be expressed in terms of those column matrices by scaling each column $X_i$ by the corresponding scalar $a_i$ and summing up the results.

`````


Geometrically, if we consider the column matrices $X_1,~X_2,~\ldots,~X_n$ as vectors in an $n$-dimensional vector space, then $V$ lies in the linear subspace spanned by these vectors when it can be expressed as their linear combination. In other words, $V$ can be represented as a combination of various directions and magnitudes given by the vectors $X_1,~X_2,~\ldots,~X_n$ in the space. The concept of linear combinations is fundamental in linear algebra and plays a central role in understanding vector spaces, spans, linear independence, and solutions to systems of linear equations.

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