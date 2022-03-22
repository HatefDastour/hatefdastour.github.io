# 1.2 Systems Of Equations, Algebraic Procedures

We start this section with an example. Consider the following system
\begin{align*}
\begin{cases}
3x_1 +2x_2 - x_3 + x_4 =-1\\
2x_1 - x_3 +2x_4 = 0\\
3x_1 + x_2 +2x_3 +5x_4 = 2
\end{cases}
\end{align*} 
This system of linear equations has three equations and four variables. We can express this in the forms of matrix (an array of numbers) as follows:

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
a_{m1}x_1+\ldots+a_{mn}x_{n}=b_m.
\end{cases}
\end{align*} 
The augmented matrix can be expressed as follows
\begin{align*}
\left[\begin{array}{cccc|c}
a_{11} & a_{12} & \dots & a_{1n} & b_{1} \\
a_{21} & a_{22} & \dots & a_{2n} & b_{2} \\
\vdots & \vdots & \ddots & \vdots & \vdots \\
a_{m1} & a_{m2} & \dots & a_{mn} & b_{m}\\
\end{array}\right]
\end{align*}
</div>


<font color='Blue'><b>Example</b></font>: Exrpess the following linear system in the augmented matrix from.

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

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***