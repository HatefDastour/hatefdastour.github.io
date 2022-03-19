# Parametric Lines

**Vector Equation of a Line**:
Suppose a line $L$ in $\mathbb{R}^n$ contains the two different points $P$ and $P_0$. Let $\vec{p}$ and $\vec{p}_0$ be the position vectors of these two points, respectively. We define $\vec{d} =\vec{p}-\vec{p}_0$ as the \textbf{direction vector} for $L$. The \textbf{vector equation} for $L$ is given by
\begin{equation*}
\vec{p} = \vec{p_0} +t\,\vec{d},\quad t \in \mathbb{R}.
\end{equation*}
In other words, the point $P$ with vector $\vec{p}$ is on this line if and only if a real number $t$ exists such
that $\vec{p} = \vec{p_0} +t\,\vec{d}$.

Consider now points in $\mathbb{R}^3$. The line through
$P_0 = (x_0 ,y_0 ,z_0 )$ with direction vector
$\vec{d}=\begin{bmatrix} a & b & c \end{bmatrix}^T\neq0$ is given by
\begin{align*}
\begin{bmatrix} x \\ y \\ z \end{bmatrix}=
\begin{bmatrix} x_0 \\ y_0 \\ z_0 \end{bmatrix}+t\begin{bmatrix} a \\ b \\ c \end{bmatrix}
\quad t \in \mathbb{R}.\end{align*} This is the vector equation of
$L$ written in **component form**.


**Parametric Equation of a Line**: The line through $P_0=(x_0 , y_0 , z_0 )$ with direction vector
$\vec{d}=\begin{bmatrix} a & b & c \end{bmatrix}^T\neq0$ is given by

\begin{align*}
\begin{cases}
x=x_0+t\,a,\\
y=y_0+t\,b,\\
z=z_0+t\,c,\\
\end{cases}
\quad t \in \mathbb{R}.\end{align*}

This is called a **parametric equation** of the line $L$.

In other words, the point $P=(x, y, z)$ is on this line if and only if a
real number t exists such that $x=x_0+t\,a$ , $y=y_0+t\,b$ , and
$z=z_0+t\,c$.

<font color='Blue'><b>Example</b></font>:
Find a vector equation for the line which contains the point $P_0 = (1,1,2)$ and has direction vector
$\vec{d} =\begin{bmatrix} 2 & 2 & 1 \end{bmatrix}^T$.
***
<font color='Green'><b>Solution</b></font>:
Letting  $P = \begin{bmatrix} x & y & z \end{bmatrix}^T$, the equation for the line is given by
\begin{align*}
\vec{p} &= \vec{p_0} +t\vec{d},\quad t \in \mathbb{R}.\\
\begin{bmatrix} x \\ y \\ z \end{bmatrix}&=
\left[\begin{array}{c} 1\\ 1\\ 2 \end{array}\right]
+t\left[\begin{array}{c} 2\\ 2\\ 1 \end{array}\right],\quad t \in \mathbb{R}.
\end{align*}
We also can write down this line in the parametric form:
\begin{align*}
\begin{cases}
x=1+2\,t,\\
y=1+2\,t,\\
z=2+t,\\
\end{cases}
\quad t \in \mathbb{R}.
\end{align*}
***

There is one other form for a line which is useful. We can solve parametric equation form for the parameter $t$,

\begin{align*}
\begin{cases}
x=x_0+t\,a,\\
y=y_0+t\,b,\\
z=z_0+t\,c,\\
\end{cases}
\quad t \in \mathbb{R},
\quad \Rightarrow{\text{Solve for $t$}}\Rightarrow
\begin{cases}
t=\dfrac{x-x_0}{a},\\
t=\dfrac{y-y_0}{b},\\
t=\dfrac{z-z_0}{c},\\
\end{cases}
\quad t \in \mathbb{R}.
\end{align*}

<div class="alert alert-block alert-success">
<p>The <strong>symmetric form</strong> of the line can be defined as follows, <span class="math display">\[\frac{x-x_0}{a}=\frac{y-y_0}{b}=\frac{z-z_0}{c}.\]</span></p>

    
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
<p>If one of <span class="math inline">\(a\)</span>, <span class="math inline">\(b\)</span>, or <span class="math inline">\(c\)</span> does happen to be zero we can still write down the symmetric equations. To see this let’s suppose that <span class="math inline">\(b=0\)</span>. In this case <span class="math inline">\(t\)</span> will not exist in the parametric equation for <span class="math inline">\(y\)</span> and so we will only solve the parametric equations for <span class="math inline">\(x\)</span> and <span class="math inline">\(z\)</span> for <span class="math inline">\(t\)</span>. We then set those equal and acknowledge the parametric equation for <span class="math inline">\(y\)</span> as follows, <span class="math display">\[\frac{x-x_0}{a}=\frac{z-z_0}{c},~y=y_0.\]</span></p>


    
</div>

<font color='Blue'><b>Example</b></font>:
Suppose the symmetric form of a line is
\begin{align*}
x-1 = \frac{y+2}{2} = \frac{z-2}{3}
\end{align*}
Write the line in parametric form as well as vector form.
***
<font color='Green'><b>Solution</b></font>:
Let $t\in \mathbb{R}$ be a parameter. Then, the parametric form can be written as follows,
\begin{align*}
\begin{cases}
x-1 =t,\\
\frac{y+2}{2} = t\\
\frac{z-2}{3}=t
\end{cases}
\quad \Rightarrow \quad 
\begin{cases}
x=t+1,\\
y=2t - 2,\\
z=3t + 2.
\end{cases}
\end{align*}
Moreover, the vector form can be found as follows,
\begin{align*}
\begin{bmatrix} x \\ y \\ z \end{bmatrix}=
\begin{bmatrix} 1 \\ -2 \\ 2 \end{bmatrix}+t\begin{bmatrix} 1 \\ 2 \\ 3 \end{bmatrix}
\quad t \in \mathbb{R}.
\end{align*}
***

<font color='Blue'><b>Example</b></font>:
Find an equation of the line through points $P_1=(2,-1,7)$ and $P_2=(-3,4,5)$ and write it in a vector form.
***
<font color='Green'><b>Solution</b></font>:
We use
\begin{equation*}
\vec{d} =\overrightarrow{P_1 P_2} =\begin{bmatrix} -3 \\4\\5 \end{bmatrix}-\begin{bmatrix} 2\\-1\\7 \end{bmatrix}=\begin{bmatrix} -5\\5\\-2 \end{bmatrix}.
\end{equation*}
Therefore,
\begin{align*}
{\text{Using }P_1} \Rightarrow \quad
\begin{bmatrix} x \\ y \\ z \end{bmatrix}&=
\begin{bmatrix} 2 \\ -1 \\ 7 \end{bmatrix}+t\begin{bmatrix} -5\\5\\-2 \end{bmatrix}
\quad t \in \mathbb{R}.
\\
\text{or}&
\\
{\text{Using }P_2} \Rightarrow \quad
\begin{bmatrix} x \\ y \\ z \end{bmatrix}&=
\begin{bmatrix} -3 \\4\\5 \end{bmatrix}+t\begin{bmatrix} -5\\5\\-2 \end{bmatrix}
\quad t \in \mathbb{R}.
\end{align*}
***

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
<p>An equation of a line is <u>not unique</u>.</p>



    
</div>

<font color='Blue'><b>Example</b></font>:
Given two lines $L_1$ and $L_2$ determine if they intersect:
$$ L_1:
\left\{ \begin{array}{rcl}
x & = & 3+t, \\
y & = & 1-2t, \\
z & = & 3+3t,
\end{array} \right.\quad (t\in \mathbb{R}),
\quad
L_2:
\left\{ \begin{array}{rcl}
x & = & 4+2s, \\
y & = & 6+3s, \\
z & = & 1+s,
\end{array} \right. \quad (s\in \mathbb{R}).
$$
***
<font color='Green'><b>Solution</b></font>:
Since at the point of intersection, the two equations will have the same values of $x$, $y$ and $z$. We set the three equations (for $x$, $y$ and $z$ in each line) equal to each other. This provides a linear system that we can solve. Let $P=(x_0,y_0,z_0)$ be the point of intersection. This means for some values of $t_0$ and $s_0$ ($t_0$ and $s_0$ are unknown and to be determined), we have
\begin{align*}
x_0 & = 3+t_0=4+2s_0\\
y_0 & = 1-2t_0=6+3s_0\\
z_0 & = 3+3t_0=1+s_0.
\end{align*}
This leads to the following linear system
\begin{align*}
\begin{cases}
2s_0-t_0=-1\\
3s_0+2t_0=-5\\
s_0-3t_0=2.
\end{cases}
\end{align*}
The augmented matrix of this system is given by
\begin{align*}
\left[\begin{array}{cc|c} 2 & -1 & -1\\3 & 2 & -5 \\1 & -3 & 2 \end{array}\right]
\quad \Rightarrow\quad{\text{In RREF}}\quad\Rightarrow\quad
\left[\begin{array}{cc|c} {1} & 0 & -1\\ 0 & {1} & -1\\ 0 & 0 & 0 \end{array}\right]
\end{align*}
Therefore, $s_0=-1$ and $t_0=-1$ and
\begin{align*}
x_0 & = 3+(-1)=2,\\
y_0 & = 1-2(-1)=3,\\
z_0 & = 3+3(-1)=0.
\end{align*}
***

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
