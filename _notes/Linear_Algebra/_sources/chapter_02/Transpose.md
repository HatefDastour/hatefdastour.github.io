# 2.1.4 Transpose

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Transpose of a Matrix
</b></font>

Transpose of a matrix is formed by
* turning rows into columns,
* turning columns into rows.

For a matrix $A$, we denote the transpose of $A$ by $A^T$.
</div>

<div class="alert alert-block alert-success">
<font size="+1"><b>
Lemma: Properties of the Transpose of a Matrix
</b></font>
    
<ul>
<li><p><span class="math inline">\(\left(A^T\right)^T=A.\)</span></p></li>
<li><p><span class="math inline">\(\left(AB\right)^T=B^TA^T.\)</span></p></li>
<li><p><span class="math inline">\(\left(rA+sB\right)^T=rA^T+sB^T.\)</span></p></li>
</ul>
    
</div>

<font color='Blue'><b>Example</b></font>: The transpose of matrix $A=\begin{bmatrix} 1 & 2 & 3 \\  4 & 5 & 6 \end{bmatrix}$ can be found as follows
\begin{equation*}
A^T=\begin{bmatrix} 1 & 2 & 3 \\  4 & 5 & 6 \end{bmatrix}^T=\begin{bmatrix} 1 & 4\\ 2 & 5\\ 3 & 6  \end{bmatrix}.
\end{equation*}

<font color='Blue'><b>Example</b></font>: Find the $A$ if
\begin{align*}
  \left(A+3 \begin{bmatrix} 1 & -1 & 0 \\  1 & 2 & 4 \end{bmatrix}\right)^T=\begin{bmatrix} 2 & 1 \\ 0 & 5 \\ 3 & 8 \end{bmatrix}.
\end{align*}

<font color='Green'><b>Solution</b></font>:
We have,
\begin{align*}
&\left(A+\begin{bmatrix} 3 & -3 & 0\\ 3 & 6 & 12 \end{bmatrix}\right)^T=\begin{bmatrix} 2 & 1 \\ 0 & 5 \\ 3 & 8 \end{bmatrix}.
\\
{\text{Transpose both sides}}\quad \Rightarrow \quad 
&\left(\left(A+\begin{bmatrix} 3 & -3 & 0\\ 3 & 6 & 12 \end{bmatrix}\right)^T\right)^T=\begin{bmatrix} 2 & 1 \\ 0 & 5 \\ 3 & 8 \end{bmatrix}^T.
\\
\Rightarrow \quad
& A+\begin{bmatrix} 3 & -3 & 0\\ 3 & 6 & 12 \end{bmatrix}=\begin{bmatrix} 2 & 0 & 3\\ 1 & 5 & 8 \end{bmatrix}.
\\
\Rightarrow \quad
& A=\begin{bmatrix} 2 & 0 & 3\\ 1 & 5 & 8 \end{bmatrix}-\begin{bmatrix} 3 & -3 & 0\\ 3 & 6 & 12 \end{bmatrix}=
\begin{bmatrix}-1 & 3 & 3\\ -2 & -1 & -4\end{bmatrix}.
\end{align*}

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
