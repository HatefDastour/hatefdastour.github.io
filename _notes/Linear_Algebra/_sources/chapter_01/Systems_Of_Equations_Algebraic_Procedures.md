# Systems Of Equations, Algebraic Procedures

Consider the following system

$$
\begin{cases}
3x_1 +2x_2 - x_3 + x_4 =-1\\
2x_1 - x_3 +2x_4 = 0\\
3x_1 + x_2 +2x_3 +5x_4 = 2
\end{cases}
$$

of three equations in four variables. The array of numbers

$$
\left[\begin{array}{cccc|c} 3 & 2 & -1 & 1 & -1\\ 2 & 0 & -1 & 2 & 0\\ 3 & 1 & 2 & 5 & 2 \end{array}\right]
$$

occurring in the system is called the **augmented matrix** of the
system.

**Augmented Matrix of a Linear System**: Suppose we have a system of equations given by

$$
\begin{cases}
a_{11}x_1+\ldots+a_{1n}x_{n}=b_1\\
a_{21}x_1+\ldots+a_{2n}x_{n}=b_2\\
\vdots \\
a_{m1}x_1+\ldots+a_{mn}x_{n}=b_m.
\end{cases}
$$

The augmented matrix of this system is given
by

$$
\left[\begin{array}{cccc|c}
a_{11} & a_{12} & \dots & a_{1n} & b_{1} \\
a_{21} & a_{22} & \dots & a_{2n} & b_{2} \\
\vdots & \vdots & \ddots & \vdots & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn} & b_{m}\\
\end{array}\right]
$$

**Elementary Operations**: The following operations, called elementary operations, can routinely be performed on systems of linear equations to produce equivalent systems.

1.  Interchange two equations.
2.  Multiply one equation by a nonzero number.
3.  Add a multiple of one equation to a different equation.

<font color='Blue'><b>Example</b></font>: Consider
$\begin{cases}x+2y =3\\x-y=0\end{cases}$. We can

1.  Interchange two equations: $\begin{cases}x-y=0\\x+2y =3\end{cases}$
2.  Multiply the first equation by 5 (a nonzero number): $\begin{cases}5x-5y=0\\x+2y =3\end{cases}$
3.  Add (-3) times of the second equation to the first equation:

\begin{align*}\begin{cases}5x-5y-3(x+2y)=0-3(3)\\x+2y =3\end{cases} &\Rightarrow \begin{cases}5x-3x-5y-6y=0-9\\x+2y =3\end{cases}
        \\&\Rightarrow \begin{cases}2x-11y=-9\\x+2y =3\end{cases}\end{align*}

In hand calculations (and in computer programs) we manipulate the rows of the augmented matrix rather than the equations.

**Elementary row operations**: The following are called elementary row operations on a matrix.

1.  Interchange two rows.
2.  Multiply one row by a nonzero number.
3.  Add a multiple of one row to a different row.


<font color='Blue'><b>Example</b></font>: First, we need to write down the system in the
augmented matrix form. We have

$$\left[\begin{array}{cc|c} 1 & 2 & 3\\1 & -1 & 0 \end{array}\right]$$

Let $R_{1}$ and $R_{2}$ denote the first row and the second row of the
current augmented matrix, respectively.

1.  Interchange the first and the second row:

    $$\left[\begin{array}{cc|c} 1 & 2 & 3\\1 & -1 & 0 \end{array}\right]
    \Rightarrow{R_{1} \leftrightarrow R_{2}}\Rightarrow
    \left[\begin{array}{cc|c} 1 & -1 & 0 \\ 1 & 2 & 3\end{array}\right]$$

2.  Multiply the first row by 5 (a nonzero number):

    $$\left[\begin{array}{cc|c} 1 & -1 & 0 \\ 1 & 2 & 3\end{array}\right]
    \Rightarrow{5 R_{1} \rightarrow R_{1}}\Rightarrow
    \left[\begin{array}{cc|c} 5 & -5 & 0 \\ 1 & 2 & 3\end{array}\right]$$

3.  Add (-3) times of the second row to the first row:

\begin{align*}
    \left[\begin{array}{cc|c} 5 & -5 & 0 \\ 1 & 2 & 3\end{array}\right]
    \Rightarrow{-3 R_{2} +R_{1} \rightarrow R_{1}}\Rightarrow
    \left[\begin{array}{cc|c} 2 & -11 & -9 \\ 1 & 2 & 3\end{array}\right]\end{align*}


```{image} ../Figures/fig1_03.png
:width: 350px
:align: center
```

<div class="alert alert-block alert-info">
<font size="+1"><b>
(Reduced) Row-Echelon Form
</b></font>
</div>

A matrix is said to be in **row-echelon form** (REF) if it satisfies the
following three conditions:

1.  All **zero rows** (consisting entirely of zeros) are at the bottom.

2.  The first nonzero entry from the left in each nonzero row is a 1,
    called the **leading 1** for that row.

3.  Each leading 1 is to the right of all leading 1 s in the rows above
    it.

A row-echelon matrix is said to be in **reduced row-echelon form**
(RREF) if, in addition, it satisfies the following condition:

4.  Each leading 1 is the only nonzero entry in its column.


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