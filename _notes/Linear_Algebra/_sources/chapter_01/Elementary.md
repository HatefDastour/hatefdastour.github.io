# 1.2.1 Elementary Operations

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Elementary Operations
</b></font>

The elementary operations can be performed on systems of linear equations to produce equivalent systems. The operations are available as follows:

1.  Interchange two equations.
1.  Multiply one equation by a nonzero number.
1.  Add a multiple of one equation to a different equation.
</div>


<font color='Blue'><b>Example</b></font>: For the following system of equations 
\begin{align*}
\begin{cases}x+2y =3\\x-y=0\end{cases}
\end{align*}
We can

1.  Interchange two equations: $\begin{cases}x-y=0\\x+2y =3\end{cases}$
1.  Multiply the first equation by 5 (a nonzero number): $\begin{cases}5x-5y=0\\x+2y =3\end{cases}$
1.  Add (-3) times of the second equation to the first equation:

\begin{align*}
\begin{cases}
5x-5y-3(x+2y)=0-3(3)\\x+2y =3\end{cases}
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

\begin{align*}
\left[\begin{array}{cc|c} 1 & 2 & 3\\1 & -1 & 0 \end{array}\right]
\end{align*}

Let $R_{1}$ and $R_{2}$ denote the first row and the second row of the
current augmented matrix, respectively.

1.  Interchange the first and the second row:

    $$\left[\begin{array}{cc|c} 1 & 2 & 3\\1 & -1 & 0 \end{array}\right]
    \Rightarrow{R_{1} \leftrightarrow R_{2}}\Rightarrow
    \left[\begin{array}{cc|c} 1 & -1 & 0 \\ 1 & 2 & 3\end{array}\right]$$

1.  Multiply the first row by 5 (a nonzero number):

    $$\left[\begin{array}{cc|c} 1 & -1 & 0 \\ 1 & 2 & 3\end{array}\right]
    \Rightarrow{5 R_{1} \rightarrow R_{1}}\Rightarrow
    \left[\begin{array}{cc|c} 5 & -5 & 0 \\ 1 & 2 & 3\end{array}\right]$$

1.  Add (-3) times of the second row to the first row:

\begin{align*}
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

a).  $\left[ \begin{array}{cc|c}
    2 & 0 & 0 \\
    0 & 1 & 1\\
    0 & 0 & 2 \\
    0 & 0 & 0 \\
    \end{array} \right]$

-   All zero rows are at the bottom. $\surd$

-   The first nonzero entry from the left in each nonzero row is not
    a 1. ${\color{red}X}$

Therefore it is not REF (If a matrix is not REF, it is not RREF as
well).


b). $ \left[ \begin{array}{ccccc|c}
1 & 3 & 0 & 5 & 0 & -1 \\
0 & 0 & 1 & 1 & 2 & 3 \\
0 & 0 & 0 & 0 & 1 & 2 \\
\end{array} \right]$

-   All zero rows are at the bottom (we don't have any all-zero rows
    here). $\surd$

-   The first nonzero entry from the left in each nonzero row is a 1.
    $\surd$

-   Each leading 1 is to the right of all leading 1 s in the rows above
    it. $\surd$

Therefore, it is a REF. However, Each leading 1 is not the only nonzero entry in its column. Therefore, it is not RREF.

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***