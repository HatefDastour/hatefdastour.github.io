# Introduction

The following textbooks were used in preparations of the notes:

1. Kuttler, Kenneth. "[A First Course in Linear Algebra (Lyryx)](https://lyryx.com/first-course-linear-algebra/)." (2021).
1. Nicholson, W. Keith. "[Linear Algebra with Applications (Lyryx)](https://lyryx.com/linear-algebra-applications/)." (2021).
1. Stewart, James, Daniel K. Clegg, and Saleem Watson. [Calculus: early transcendentals](https://books.google.ca/books/about/Calculus_Early_Transcendentals.html). Cengage Learning, 2020.


Throughout Chapter 1 of the textbook, A First Course in Linear Algebra by K. Kuttler {cite}`kuttler2017first`, there are several notations and terminologies that are introduced from Chapter 2 onwards. Therefore, in this prologue, we set the stage by briefly discussing some points of notation and terminology that will be used throughout this semester.

## Equation
<div class="alert alert-info" role="alert">
<font size="+1"><b>
Equation
</b></font>

<p style='text-align: justify;'>
In an equation, there is an equal sign (=), and the two sides of this equal sign are called equal. There is at least one unknown value which is known as a variable.
</p>
</div>

For example,

\begin{align*}
x+2=3
\end{align*} 

is a mathematical equation where $x$ is a variable (an unknown value).

## Planes

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Plane
</b></font>

<p style='text-align: justify;'>
A plane is a zero thickness surface with an infinitely large area.
</p>
</div>

We will discuss planes more in Chapter 4.

For two planes in three-dimensional space, we can have either **parallel planes** or **intersecting planes**.

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Parallel planes
</b></font>

<p style='text-align: justify;'>
The distance between parallel planes is always the same, and they never have any intersections.
</p>

```{image} Figures/fig0_01.png
:width: 400px
:align: center
```
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Intersecting planes
</b></font>

<p style='text-align: justify;'>
If two planes are not parallel (the distance between them is not always the same), they will have an intersection. The intersection of two planes always happens in the form of a line.
</p>

```{image} Figures/fig0_02.png
:width: 300px
:align: center
```
</div>

<div class="alert alert-warning" role="alert">
Note that two planes intersect at a line, and two lines intersect at a point.
</div>


<div class="alert alert-info" role="alert">
<font size="+1"><b>
Hyperplane
</b></font>
<p style='text-align: justify;'>
A hyperplane is a plane with one less dimension than the dimension of its ambient space. For example, if space is 3-dimensional, then its hyperplanes are 2-dimensional planes. Moreover, if the space is 2-dimensional, its hyperplanes are the 1-dimensional lines.
</p>
</div>

## Matrix
<div class="alert alert-info" role="alert">
<font size="+1"><b>
Matrix
</b></font>
A matrix is a mathematical way of presenting a set of numbers in a  tabular form (in rows and columns). A matrix can contain real numbers such as $1$, $5$, $\sqrt{2}$, $\frac{2}{3}$, ..., or complex numbers such as $1+i$, $i$, $1-i$, ....
</div>


Here is an example of a matrix with four rows and three columns:

```{image} Figures/fig0_03.png
:width: 600px
:align: center
```

<div class="alert alert-warning" role="alert">
<font size="+1"><b>
Remarks
</b></font>

1.  Each number from a matrix is called an **element** or an **entry** of the matrix. The elements (entries) in a matrix have indices that refer to their specific locations. For example, the upper left corner of the matrix is the first row (or simply, \textbf{row 1}) and the first column (or simply, \textbf{column 1}). The entry at row 1 and column 1 is 1. Similarly, the entry at row 4 and column 4 is 11.

2.  A matrix with $m$ rows and $n$ columns is referred to as an $m\times n$ matrix or as having size $m\times n$. For example, $A=\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 &9 \\ 10 & 11 & 12 \end{bmatrix}$ is a $4\times 3$ matrix (it has four rows and three columns).

3.  $A$ matrix of size $1\times n$ is called a **row matrix** (it just has a row), whereas one of size $m\times1$ is called a **column matrix** (it has only a column). For example, $\begin{bmatrix} 1 & 2 & 3\end{bmatrix}$ is a row matrix and $\begin{bmatrix} 1 \\ 2 \\ 3\end{bmatrix}$ is a column matrix.

4.  A **square matrix** has the same number of rows and columns. For example, $\begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}$ and
    $\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 &9\end{bmatrix}$ are $2\times 2$ and $3\times 3$ square matrices, respectively.

5.  **Scalar multiplication of matrices**: If $A$ is a matrix and $k$ is a scalar (a scalar is just a number, such as $2$, $3$,
    $\frac{5}{2}$,...), then $kA$ is also a matrix whose entries are multiplied by $k$. See the following examples:
    
	$$\begin{aligned}
    2\begin{bmatrix} 1 \\ 2 \\ 3\end{bmatrix}=\begin{bmatrix} (2)(1) \\ (2)(2) \\ (2)(3)\end{bmatrix}
    =\begin{bmatrix} 2 \\ 4 \\ 6\end{bmatrix}
    \quad \text{ and } \quad
    2\begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}=\begin{bmatrix} (2)(1) & (2)(2) \\ (2)(3) & (2)(4) \end{bmatrix}
    =\begin{bmatrix} 2 & 4 \\ 6 & 8\end{bmatrix}.\end{aligned}$$
</div>

```{bibliography}
:style: alpha
```