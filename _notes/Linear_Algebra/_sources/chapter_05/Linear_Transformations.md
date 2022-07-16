# Linear Transformations

## Transformation

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Transformation
</b></font>

A function from $\mathbb{R}^n$ to $\mathbb{R}^m$ is called a **transformation from $\R^n$ to $\R^m$**, and it can be written as
follows 
\begin{aligned}\mathbb{R}^n\stackrel{T}{\rightarrow} \mathbb{R}^m.\end{aligned}
Here, **$T$ is a transformation of $\mathbb{R}^n$** if $m = n$.

</div>


<font color='Blue'><b>Example</b></font>:
Consider the matrix $A = \left[
\begin{array}{rrr}
1 & 0 & 1\\ 2 & 2 & 1
\end{array}
\right]$. By matrix multiplication, $A$ transforms vectors in $\mathbb{R}^3$ into vectors in $\mathbb{R}^2$.

Consider the vector $\left[
\begin{array}{c}
x \\
y \\
z
\end{array}
\right]$. Transforming this vector by $A$ looks like:
\begin{align*}
\left[\begin{array}{rrr} 1 & 0 & 1\\ 2 & 2 & 1\end{array}\right]\left[\begin{array}{c}x \\y \\z\end{array}\right]
=\left[\begin{array}{c}x + z \\2x + 2y+z\end{array}\right]
\end{align*}

If $T$ acts by matrix multiplication of a matrix $A$ (such as the
previous example), we call $T$ a **matrix transformation**, and write
$T_A(\vec{x}) = A\vec{x}$. The matrix transformation of vector $\vec{x}$
is written as follows. \begin{align*}
T_A (\vec{x}) = A\vec{x}\end{align*}

In the previous example, a linear transformation from $\mathbb{R}^3$
into $\mathbb{R}^2$: \begin{align*}
\begin{cases}
T:~\mathbb{R}^3 \to \mathbb{R}^2,\\
T_A (\vec{x}) = A\vec{x},
\end{cases}\end{align*} where
$A=\begin{bmatrix}1 & 0 & 1\\ 2 & 2 & 1\end{bmatrix}$. This
transformation can for example transform
$\begin{bmatrix}1\\ 2\\ 3\end{bmatrix}$ into
$\begin{bmatrix}4\\ 9\end{bmatrix}$ \begin{align*}
\begin{bmatrix}1 & 0 & 1\\ 2 & 2 & 1\end{bmatrix}\begin{bmatrix}1\\ 2\\ 3\end{bmatrix}=\begin{bmatrix}4\\ 9\end{bmatrix}\end{align*}

## Linear Transformation

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Linear Transformation
</b></font>

A transformation $T:\mathbb{R}^n\rightarrow \mathbb{R}^m$ is a **linear
transformation** if it satisfies the following two properties for all
$\vec{x},\vec{y}\in\mathbb{R}^n$ and all (scalars) $k\in\mathbb{R}$.\


1. $T(\vec{x}+\vec{y})=T(\vec{x})+T(\vec{y})$ (preservation of
    addition)

2. $T(k\vec{x})=kT(\vec{x})$ (preservation of scalar multiplication)

</div>

Some important examples of linear transformations are the **zero transformation** and **identity transformation**. The zero transformation defined by $T (\vec{x}) = \vec{0}$ for all $\vec{x}$ is an example of a linear transformation. Similarly, the identity transformation defined by $T (\vec{x}) = \vec{x}$ is also linear.

<font color='Blue'><b>Example</b></font>:
\begin{align*}
\begin{array}{lc}
\text{Identity transformation:} & T:~\mathbb{R}^3 \to \mathbb{R}^3 \text{ is defined by } T\begin{bmatrix}x_1\\ x_2\\ x_3\end{bmatrix}=\begin{bmatrix}x_1\\ x_2\\ x_3\end{bmatrix},
\\
\text{Zero transformation:} & T:~\mathbb{R}^3 \to \mathbb{R}^3 \text{ is defined by }T\begin{bmatrix}x_1\\ x_2\\ x_3\end{bmatrix}=\begin{bmatrix}0\\ 0\\ 0\end{bmatrix}.
\end{array}
\end{align*}

<font color='Blue'><b>Example</b></font>:
Let $T$ be a transformation defined by $T:~\mathbb{R}^3 \to \mathbb{R}^2$ is defined by
\begin{align*}
T\begin{bmatrix}x_1\\ x_2\\ x_3\end{bmatrix}=\begin{bmatrix}x_{1}+x_{3}\\ 2\,x_{1}+2\,x_{2}+x_{3}\end{bmatrix}
\end{align*}
Show that $T$ is a linear transformation.

<font color='Green'><b>Solution</b></font>: 
Let $\vec{y}=\begin{bmatrix}y_1\\ y_2\\ y_3\end{bmatrix}$ and
$\vec{z}=\begin{bmatrix}z_1\\ z_2\\ z_3\end{bmatrix}$ be two vectors in
$\mathbb{R}^3$. We have

1.  $$\begin{aligned}
    T\left(\vec{y}+\vec{z} \right)&=
    T\left(\begin{bmatrix}y_1\\ y_2\\ y_3\end{bmatrix}+\begin{bmatrix}z_1\\ z_2\\ z_3\end{bmatrix}\right)=T\,\begin{bmatrix}y_1+z_1\\ y_2+z_2\\ y_3+z_3\end{bmatrix}
	\\ &
    =\begin{bmatrix}y_{1}+z_{1}+y_{3}+z_{3}\\ 2\,(y_{1}+z_{1})+2\,(y_{2}+z_{2})+y_{3}+z_{3}\end{bmatrix}
    \\ &
    =\begin{bmatrix}y_{1}+y_{3}\\ 2\,y_{1}+2\,y_{2}+y_{3}\end{bmatrix}+\begin{bmatrix}z_{1}+z_{3}\\ 2\,z_{1}+2\,z_{2}+z_{3}\end{bmatrix}
    =T\left(\vec{y}\right)+T\left(\vec{z} \right).\end{aligned}$$

2.  For any scalar $k\in \mathbb{R}$, $$\begin{aligned}
    T \left(k\,\vec{y}\right) &=T\left(k\begin{bmatrix}y_1\\ y_2\\ y_3\end{bmatrix}\right)
    =T\begin{bmatrix}ky_1\\ ky_2\\ ky_3\end{bmatrix}
    =\begin{bmatrix}ky_{1}+ky_{3}\\ 2k\,y_{1}+2k\,y_{2}+ky_{3}\end{bmatrix}
    \\ &
    =k\begin{bmatrix}y_{1}+y_{3}\\ 2\,y_{1}+2\,y_{2}+y_{3}\end{bmatrix}
    =k\,T \left(\vec{y}\right).\end{aligned}$$

Therefore, $T$ is a linear transformation.
***
## Matrix Transformations are Linear Transformations
<div class="alert alert-info" role="alert">
<font size="+1"><b>
Matrix Transformations are Linear Transformations
</b></font>

Every linear transformation can be expressed as a matrix transformation. if $T :~\mathbb{R}^n \to \mathbb{R}^m$ is a linear transformation , then it can be written as $T(\vec{x}) = A\vec{x}$, where $A$ is a matrix.
</div>


***
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
