# The Matrix of a Linear Transformation

If $T$ is any linear transformation which maps $\mathbb{R}^n$ to $\mathbb{R}^m$, there is \textbf{always} an $m\times n$ matrix $A$ with the property that
\begin{align*}
T(\vec{x}) = A \vec{x},\quad \text{for all }x\in \mathbb{R}^n.
\end{align*}

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: Matrix of a Linear Transformation
</b></font>
    
If $T$ is any linear transformation which maps $\mathbb{R}^n$ to $\mathbb{R}^m$, there is **always** an $m\times n$ matrix $A$ with the property that
\begin{align*}
T(\vec{x}) = A \vec{x},\quad \text{for all }x\in \mathbb{R}^n.
\end{align*}

</div>

Let $T :~\mathbb{R}^n \to \mathbb{R}^m$ be a linear transformation, and we want to identify the matrix defined by this linear transformation $T(\vec{x}) = A \vec{x}$. Note that for any $\vec{x}\in \mathbb{R}^n$,

\begin{align*}
\vec{x}=
\begin{bmatrix}x_1\\x_2\\x_3\\ \vdots \\x_n\end{bmatrix}
&=x_1\begin{bmatrix}1\\0\\0\\ \vdots \\0\end{bmatrix}+x_2\begin{bmatrix}0\\1\\0\\ \vdots \\0\end{bmatrix}+\ldots
+x_n\begin{bmatrix}0\\0\\0\\ \vdots \\1\end{bmatrix}
%\\ &
=x_1 \vec{e}_1+x_2 \vec{e}_2+\ldots+x_n \vec{e}_n
\end{align*}
where where $\vec{e}_i$ is the $i^{\text{th}}$ column of $I_n$. Then, since $T$ is linear,
\begin{align*}
T\left(\vec{x}\right)&=T\left(x_1 \vec{e}_1+x_2 \vec{e}_2+\ldots+x_n \vec{e}_n\right)=
x_1 T\left(\vec{e}_1\right)+x_2 T\left(\vec{e}_2\right)+\ldots+x_n T\left(\vec{e}_n\right)
\\ &
=\begin{bmatrix}| & | & \dots & |\\T\left(\vec{e}_1\right) & T\left(\vec{e}_2\right) & \dots & T\left(\vec{e}_n\right)\\
| & | & \dots & | \end{bmatrix} \begin{bmatrix}x_1\\x_2\\x_3\\ \vdots \\x_n\end{bmatrix}
=A\,\begin{bmatrix}x_1\\x_2\\x_3\\ \vdots \\x_n\end{bmatrix}=A\,\vec{x}.
\end{align*}

<font color='Blue'><b>Example</b></font>:
Let $T$ be a linear transformation defined by $T:~\mathbb{R}^3 \to \mathbb{R}^4$ is defined by
\begin{align*}
T\begin{bmatrix}a\\b\\c\end{bmatrix}=\begin{bmatrix}a+b-3c\\b+c\\a-c\\2a-b+c\end{bmatrix}.
\end{align*}
Find $A$ so that $T(\vec{x}) = A\vec{x}$.

<font color='Green'><b>Solution</b></font>:
First, let's find $T\left(\vec{e}_1\right)$, $T\left(\vec{e}_2\right)$ and $T\left(\vec{e}_3\right)$.
\begin{align*}
&T\left(\vec{e}_1\right)=T\begin{bmatrix}1\\0\\0\end{bmatrix}=\begin{bmatrix}1+0-3(0)\\0+0\\1-0\\2(1)-0+0\end{bmatrix}=
\begin{bmatrix}1\\0\\1\\2\end{bmatrix},
\\
&T\left(\vec{e}_2\right)=T\begin{bmatrix}0\\1\\0\end{bmatrix}=\begin{bmatrix}0+1-3(0)\\1+0\\0-0\\2(0)-1+0\end{bmatrix}=
\begin{bmatrix}1\\1\\0\\-1\end{bmatrix},
\\
&T\left(\vec{e}_3\right)=T\begin{bmatrix}0\\0\\1\end{bmatrix}=\begin{bmatrix}0+0-3(1)\\0+1\\0-1\\2(0)-0+1\end{bmatrix}=
\begin{bmatrix}-3\\1\\-1\\1\end{bmatrix}.
\end{align*}
Moreover, we can find matrix $A$ as follows
\begin{equation*}
A=\begin{bmatrix}| & | & |\\T\left(\vec{e}_1\right) & T\left(\vec{e}_2\right) & T\left(\vec{e}_3\right)\\| & | & |\end{bmatrix}
=\begin{bmatrix} 1 & 1 & -3\\0 & 1 & 1\\ 1 & 0 & -1\\ 2 & -1 & 1\end{bmatrix}
\end{equation*}
***

<div class="alert alert-block alert-success">
<font size="+1"><b>
Corollary: Matrix and Linear Transformation
</b></font>
    
A transformation $T$ from $\mathbb{R}^n$ to $\mathbb{R}^m$, i.e. $T :~\mathbb{R}^n \to \mathbb{R}^m$, is a linear transformation if and only if it is a matrix transformation.

</div>

***
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
