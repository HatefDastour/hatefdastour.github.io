# 1.2.2 Gaussian Elimination


<div class="alert alert-info" role="alert">
<font size="+1"><b>
Equivalent Matrices
</b></font>

The matrix $B$ is equivalent to the matrix $A$ if $B$ can be obtained from $A$ by performing a sequence of elementary row operations starting with $A$.
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem:
</b></font>

* If corresponding augmented matrices of two linear systems of equations are equivalent, then those two linear systems have exactly the same solutions.
* Every matrix $A$ is equivalent to a unique matrix in RREF.
</div>

<div class="alert alert-block alert-success">
<font size="+1"><b>
Gaussian Algorithm:
</b></font>
<p><strong>Step 1</strong>: If the matrix consists entirely of zeros, stop. It is already in row-echelon form.</p>
<p><strong>Step 2</strong>: Otherwise, find the first column from the left containing a nonzero entry (call it <span class="math inline">\(a\)</span>), and move the row containing that entry to the top position.</p>
<p><strong>Step 3</strong>: Now multiply the new top row by <span class="math inline">\(1/a\)</span> to create a leading 1 .</p>
<p><strong>Step 4</strong>: By subtracting multiples of that row from rows below it, make each entry below the leading 1 zero. This completes the first row, and all further row operations are carried out on the remaining rows.</p>
<p><strong>Step 5</strong>: Repeat steps 1-4 on the matrix consisting of the remaining rows. The process stops when either no rows remain at step 5 or the remaining rows consist entirely of zeros.</p>
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Back-Substitution
</b></font>

Back-substitution is a process of solving a linear system of equations using its transformed into a row-echelon form or the reduced row-echelon form. In this process, the last equation is solved first, then the second last equation is solved next, etc.
</div>

<font color='Blue'><b>Example</b></font>: Solve the following linear system using back-substitution.
\begin{equation*}
\begin{cases}
x_{1}+2\,x_{2}+3\,x_{3}=2\\
4\,x_{1}-3\,x_{2}+x_{3}=-3\\
x_{2}-2\,x_{1}+3\,x_{3}=5
\end{cases}
\end{equation*}

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

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***