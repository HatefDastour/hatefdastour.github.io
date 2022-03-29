# 4.9 The Cross Product

## Right Hand System of Vectors
<div class="alert alert-info" role="alert">
<font size="+1"><b>
Right Hand System of Vectors
</b></font>

Three vectors, $\vec{u}$, $\vec{v}$, $\vec{w}$ form a right-hand system if when you extend the fingers of your right hand along the direction of vector $\vec{u}$ and close them in the direction of $\vec{v}$, the thumb points roughly in the direction of $\vec{w}$.

```{image} ../Figures/fig4_37.png
:width: 200px
:align: center
```
</div>

For an example of a right handed system of vectors, see the following picture.
```{image} ../Figures/fig4_20.png
:width: 160px
:align: center
```


In this picture the vector $\vec{w}$ points upwards from the plane determined by the other two vectors. Point the fingers of your right hand along $\vec{u}$, and close them in the direction of $\vec{v}$. Notice that if you extend the thumb on your right hand, it points in the direction of $\vec{w}$.

```{image} ../Figures/fig4_37.png
:width: 160px
:align: center
```

Try using your left hand and you will see that the vector $\vec{w}$ would need to point in the opposite direction.

```{image} ../Figures/fig4_38.png
:width: 160px
:align: center
```

## Coordinate Vectors
<div class="alert alert-info" role="alert">
<font size="+1"><b>
Coordinate Vectors
</b></font>

The coordinate vectors are unit vectors in the direction of the $x$, $y$, and $z$ axes of a three dimensional Cartesian coordinate system.
\begin{align*}
\vec{i}=\begin{bmatrix}1\\0\\0\end{bmatrix},\quad \vec{j}=\begin{bmatrix}0\\1\\0\end{bmatrix} ,\quad \text{and}\quad  \vec{k}=\begin{bmatrix}0\\0\\1\end{bmatrix}.
\end{align*}

```{image} ../Figures/fig4_21.png
:width: 280px
:align: center
```
</div>


<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
Note that the special vectors, $\vec{i}$, $\vec{j}$, $\vec{k}$ will always form a right handed system. If you extend the fingers
of your right hand along $\vec{i}$ and close them in the direction $\vec{j}$, the thumb points in the direction of $\vec{k}$.

```{image} ../Figures/fig4_22.png
:width: 450px
:align: center
```
</div>

## Geometric Definition of Cross Product
<div class="alert alert-info" role="alert">
<font size="+1"><b>
Geometric Definition of Cross Product
</b></font>

Let $\vec{u}$ and $\vec{v}$ be two vectors in $\mathbb{R}^3$. Then the
cross product, written $\vec{u}\times \vec{v}$, is defined by the
following two rules:

1.  Its length is
    $\|\vec{u}\times \vec{v}\| = \|\vec{u}\|\|\vec{v}\|\sin(\theta)$,
    where $\theta$ is the included angle between $\vec{u}$ and
    $\vec{v}$.

2.  It is perpendicular to both $\vec{u}$ and $\vec{v}$, that is
    $(\vec{u}\times\vec{v})\bullet \vec{u} = 0$,
    $(\vec{u}\times\vec{v})\bullet \vec{v} = 0$, and $\vec{u}$,
    $\vec{v}$, $\vec{u}\times\vec{v}$ form a right hand system.
    
```{image} ../Figures/fig4_25.png
:width: 240px
:align: center
```
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
The dot product of two vectors results in a **scalar** (a number) as opposed to the cross product that results in a vector (has direction
and magnitude).    
</div>

<div class="alert alert-block alert-success">

The cross product of the special vectors $\vec{i}$, $\vec{j}$ and $\vec{k}$ is as follows.

\begin{align*}
\begin{array}{cc}
\vec{i}\times \vec{j} = \vec{k}, & \vec{j}\times \vec{i} = - \vec{k} \\
\vec{k} \times \vec{i} = \vec{j}, & \vec{i}\times \vec{k} = - \vec{j} \\
\vec{j}\times \vec{k} = \vec{i}, & \vec{k}\times \vec{j} = - \vec{i}  \\
\end{array}
\end{align*} 
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
Not that a vector $\vec{u} =\begin{bmatrix}u_1 & u_2  &u_3\end{bmatrix}^T$ can be written in terms of  $\vec{i}$, $\vec{j}$ and $\vec{k}$ as \begin{align*}\vec{u}= u_1 \vec{i}+u_2\vec{j}+u_3 \vec{k}.\end{align*}     
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Proposition: Coordinate Description of Cross Product
</b></font>
    
Let $\vec{u}= u_1 \vec{i}+u_2\vec{j}+u_3 \vec{k}$ and $\vec{v} = v_1 \vec{i}+v_2\vec{j}+v_3\vec{k}$ be two vectors. Then
\begin{align*}
\vec{u} \times \vec{v} &=\begin{bmatrix}u_2 v_3 -u_3 v_2\\-(u_1v_3 -u_3 v_1 )\\u_1 v_2 -u_2 v_1\end{bmatrix}\\
&=(u_2 v_3 -u_3 v_2)\vec{i}-(u_1v_3 -u_3 v_1 )\vec{j}+(u_1 v_2 -u_2 v_1)\vec{k}
\end{align*}    
</div>

We also can express the cross product as the determinant of a matrix,
\begin{align*}
\vec{u} \times \vec{v} &=
\left|\begin{array}{ccc} \vec{i} & \vec{j} & \vec{k}\\u_1 & u_2 & u_3 \\ v_1 & v_2 & v_3 \end{array}\right|
%\\&
=\vec{i} \left|\begin{array}{cc}  u_2 & u_3 \\v_2 & v_3\end{array}\right|
-\vec{j} \left|\begin{array}{cc} u_1 & u_3 \\v_1 & v_3\end{array}\right|
+\vec{k} \left|\begin{array}{cc} u_1 & u_2 \\v_1 & v_2\end{array}\right|\\
&=(u_2 v_3 -u_3 v_2)\vec{i}-(u_1v_3 -u_3 v_1 )\vec{j}+(u_1 v_2 -u_2 v_1)\vec{k}
\end{align*}

## Properties of the Cross Product
<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Proposition: Properties of the Cross Product
</b></font>
    
Let $\vec{u}$, $\vec{v}$, $\vec{w}$ be vectors in $\mathbb{R}^3$, and $k$ a scalar. Then, the following properties of the cross product hold.
1. $\vec{u}\times \vec{v} = -(\vec{v}\times \vec{u})$, and $\vec{u}\times \vec{u}=0$,
2. $(k\vec{u})\times \vec{v} = k(\vec{u}\times \vec{v}) = \vec{u}\times (k\vec{v})$,
3. $\vec{u}\times (\vec{v}+\vec{w}) = \vec{u}\times \vec{v}+\vec{u}\times  \vec{w}$,
4. $(\vec{v}+\vec{w})\times \vec{u}=\vec{v}\times \vec{u}+\vec{w}\times \vec{u}$.
</div>

<font color='Blue'><b>Example</b></font>: Find $\vec{u}\times \vec{v}$ and $\vec{v}\times \vec{u}$ for the following vectors $\vec{u}=\begin{bmatrix} 2\\0\\-2 \end{bmatrix}$ and
$\vec{v}=\begin{bmatrix} 0\\5\\3 \end{bmatrix}$.

<font color='Green'><b>Solution</b></font>: 
\begin{align*}
\vec{u} \times \vec{v} &=
\left|\begin{array}{ccc} \vec{i} & \vec{j} & \vec{k}\\ 2 & 0 & -2  \\ 0 & 5 & 3  \end{array}\right|
=\vec{i} \left|\begin{array}{cc}  0 & -2 \\ 5 & 3\end{array}\right|
-\vec{j} \left|\begin{array}{cc} 2 & -2 \\ 0 & 3\end{array}\right|
+\vec{k} \left|\begin{array}{cc} 2 & 0 \\ 0 & 5\end{array}\right|=10\vec{i}-6\vec{j}+10\vec{k},
\\
\vec{v} \times \vec{u} &=
\left|\begin{array}{ccc} \vec{i} & \vec{j} & \vec{k}  \\ 0 & 5 & 3 \\ 2 & 0 & -2 \end{array}\right|
=\vec{i} \left|\begin{array}{cc}  5 & 3\\ 0 & -2\end{array}\right|
-\vec{j} \left|\begin{array}{cc} 0 & 3\\ 2 & -2\end{array}\right|
+\vec{k} \left|\begin{array}{cc}  0 & 5\\ 2 & 0\end{array}\right|=-10\vec{i}+6\vec{j}-10\vec{k}.
\end{align*}

***
<font color='Blue'><b>Example</b></font>: 
Let $A = (0,0,1)$, $B = (2,0,-1)$ and $C = (0,1,0)$ be point in $\mathbb{R}^3$. Find an equation for the plane containing $A$, $B$, and $C$.

<font color='Green'><b>Solution</b></font>:
```{image} ../Figures/fig4_26.png
:width: 320px
:align: center
```

The vectors $\overrightarrow{AB}$ and $\overrightarrow{AC}$ lie in the plane; therefore,
\begin{align*}
\overrightarrow{AB}=
\begin{bmatrix} 2 \\ 0 \\ -1  \end{bmatrix}-\begin{bmatrix} 0 \\ 0 \\ 1  \end{bmatrix}=\begin{bmatrix} 2 \\ 0 \\ -2 \end{bmatrix}
\quad \text{and}\quad
\overrightarrow{AC}=
\begin{bmatrix} 0 \\ 1 \\ 0  \end{bmatrix}-\begin{bmatrix} 0 \\ 0 \\ 1  \end{bmatrix}=\begin{bmatrix} 0 \\ 1 \\ -1 \end{bmatrix}
\end{align*}
and
\begin{align*}
\vec{n}&=\overrightarrow{AB} \times \overrightarrow{AC} =
\left|\begin{array}{ccc} \vec{i} & \vec{j} & \vec{k}\\ 2 & 0 & -2 \\ 0 & 1 & -1 \end{array}\right|
%\\&
=\vec{i} \left|\begin{array}{cc}  0 & -2\\ 1 & -1 \end{array}\right|
-\vec{j} \left|\begin{array}{cc} 2 & -2\\ 0 & -1 \end{array}\right|
+\vec{k} \left|\begin{array}{cc}  2 & 0\\ 0 & 1 \end{array}\right|\\
&=2\vec{i}+2\vec{j}+2\vec{k}
\end{align*}
is a normal for the plane (being orthogonal to both $\overrightarrow{AB}$ and $\overrightarrow{AC}$).
Since all three points $A$, $B$ and $C$ are on the plane, we can use any of them to write down an equation of the plan. Hence the plane has equation

\begin{align*}
\text{Using }A = (0,0,1) \quad\Rightarrow \quad & 2(x-0)+2(y-0)+2(z-1) = 0\\
\text{Simplifying}  \quad\Rightarrow \quad & 2x+2y+2z -2 = 0\\
\text{Moving -2 to the RHS} \quad\Rightarrow \quad & 2x+2y+2z =2\\
\text{Dived both sides by 2} \quad\Rightarrow \quad & x+y+z =1.
\end{align*}

An important geometrical application of the cross product is as follows. The size of the cross product, $\|\vec{u}\times \vec{v}\|$, is the area of the parallelogram determined by $\vec{u}$ and $\vec{v}$.

```{image} ../Figures/fig4_27.png
:width: 320px
:align: center
```

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Proposition: The Area of a Parallelogram and The Area of a Triangle
</b></font>
    
Let $\vec{u}$ and $\vec{v}$ be three vectors in $\mathbb{R}^n$:
* Area of a Parallelogram = $\|\vec{u}\times \vec{v}\| = \|\vec{u}\|\|\vec{v}\|\sin(\theta)$,
```{image} ../Figures/fig4_28.png
:width: 300px
:align: center
```
* Area of a Triangle = $\dfrac{1}{2}\|\vec{u}\times \vec{v}\| = \dfrac{1}{2}\|\vec{u}\|\|\vec{v}\|\sin(\theta)$.
```{image} ../Figures/fig4_29.png
:width: 240px
:align: center
```
where $\theta$ is the included angle between $\vec{u}$ and $\vec{v}$.
</div>

<font color='Blue'><b>Example</b></font>:
Find the area of the parallelogram determined by the vectors $\begin{bmatrix} 1 & 2 & 3 \end{bmatrix}^T$ , $\begin{bmatrix} 3 & -2 &1\end{bmatrix}^T$.

<font color='Green'><b>Solution</b></font>: 
Let $\begin{bmatrix} 1 & 2 & 3 \end{bmatrix}^T$ and $\begin{bmatrix} 3 & -2 &1\end{bmatrix}^T$. The area can be found as follows,
\begin{align*}
\vec{u}\times \vec{v}&=
\left|\begin{array}{ccc} \vec{i} & \vec{j} & \vec{k}\\ 1 & 2 & 3\\ 3 & -2 & 1 \end{array}\right|
=\begin{bmatrix} 8\\ 8\\ -8 \end{bmatrix}\\
\Rightarrow \|\vec{u}\times \vec{v}\|&=\sqrt{64+64+64}=\sqrt{3\times 64}=8\sqrt{3}.
\end{align*}

***
<font color='Blue'><b>Example</b></font>:
Find the area of the triangle having vertices $A(3,-1,2)$, $B(1,1,0)$ and $C(1,2,-1)$.

<font color='Green'><b>Solution</b></font>: 
The area of the triangle is half the area of the parallelogram defined by $\overrightarrow{AB}$ and $\overrightarrow{AC}$.
\begin{align*}
\overrightarrow{AB}=\begin{bmatrix} -2 \\ 2 \\ -2 \end{bmatrix}\quad \text{and}\quad \overrightarrow{AC}=\begin{bmatrix} -2 \\ 3 \\ -3 \end{bmatrix}
\end{align*}
Therefore,
\begin{align*}
\overrightarrow{AB}\times \overrightarrow{AC}=
\left|\begin{array}{ccc} \vec{i} & \vec{j} & \vec{k}\\ -2 & 2 & -2\\ -2 & 3 & -3 \end{array}\right|
=\begin{bmatrix} 0 \\ -2 \\ -2\end{bmatrix}
\end{align*}
As a result, the area of the triangle is
\begin{align*}
\frac{1}{2}\|\overrightarrow{AB}\times \overrightarrow{AC}\|=\frac{1}{2}\sqrt{0+4+4}=\frac{1}{2}\sqrt{4\times 2}=\sqrt{2}
\end{align*}

If the two vectors $\vec{u}$ and $\vec{v}$ are parallel then the angle between them is either $0$ or $\pi$ degrees.
$\|\vec{u}\times \vec{v}\| = \|\vec{u}\|\|\vec{v}\|\sin(\theta)$ implies that $\|\vec{u}\times \vec{v}\|=0$.

<div class="alert alert-block alert-success">
<font size="+1"><b>
Lemma:
</b></font>
    
<p>If <span class="math inline">\(\vec{u}\times \vec{v}=\vec{0}\)</span>, <span class="math inline">\(\vec{u}\)</span> and <span class="math inline">\(\vec{v}\)</span> are parallel vectors.</p>

    
</div>

<font color='Blue'><b>Example</b></font>:
Determine whether $\vec{u}=\begin{bmatrix} 1&1&-1 \end{bmatrix}^T$ and $\vec{v}=\begin{bmatrix} 1&0&2 \end{bmatrix}^T$  are parallel.

<font color='Green'><b>Solution</b></font>: 
\begin{align*}
\vec{u}\times \vec{v}&=
\left|\begin{array}{ccc} \vec{i} & \vec{j} & \vec{k}\\ 1 & 1 & -1\\ 1 & 0 & 2 \end{array}\right|
=\begin{bmatrix} 2\\ -3\\ -1 \end{bmatrix}\neq \begin{bmatrix} 0\\ 0\\ 0\end{bmatrix}.
\end{align*}
$\vec{u}$ and $\vec{v}$ are **not parallel**.

## The Box Product
<div class="alert alert-info" role="alert">
<font size="+1"><b>
The Box Product
</b></font>

\begin{align*}
(\vec{u}\times \vec{v})\bullet \vec{w}=\|\vec{u}\times \vec{v}\|\|\vec{w}\|\cos(\theta).
\end{align*}
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Proposition: 
</b></font>
    
<p>Let <span class="math inline">\(\vec{u}\)</span>, <span class="math inline">\(\vec{v}\)</span>, <span class="math inline">\(\vec{w}\)</span> be vectors. Then <span class="math inline">\((\vec{u}\times \vec{v})\bullet \vec{w}=\vec{u}\bullet( \vec{v}\times \vec{w})\)</span>.</p>

    
</div>

<div class="alert alert-block alert-success">
<p>Let <span class="math inline">\(\vec{u}\)</span>, <span class="math inline">\(\vec{v}\)</span>, <span class="math inline">\(\vec{w}\)</span> be three vectors in <span class="math inline">\(\mathbb{R}^n\)</span> that define a parallelepiped. Then the volume of theparallelepiped is the absolute value of the box product, given by <span class="math display">\[|(\vec{u}\times \vec{v})\bullet \vec{w}|.\]</span></p>

```{image} ../Figures/fig4_30.png
:width: 320px
:align: center
```
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
<p>Given <span class="math inline">\(\vec{u}= u_1 \vec{i}+u_2\vec{j}+u_3 \vec{k}\)</span>, <span class="math inline">\(\vec{v} = v_1 \vec{i}+v_2\vec{j}+v_3\vec{k}\)</span> and <span class="math inline">\(\vec{w} = w_1 \vec{i}+w_2\vec{j}+w_3\vec{k}\)</span>: <span class="math display">\[\begin{aligned}
\vec{u}\bullet( \vec{v}\times \vec{w}) &=
\left|\begin{array}{ccc} u_1 & u_2 & u_3 \\ v_1 & v_2 & v_3\\ w_1 & w_2 & w_3 \end{array}\right|\end{aligned}\]</span></p>

    
</div>

<font color='Blue'><b>Example</b></font>:
Find the volume of the parallelepiped determined by the vectors $\vec{u}=\begin{bmatrix} 1 & 0 & 0 \end{bmatrix}^T$,
$\vec{v}=\begin{bmatrix} 0 & 1 & 0 \end{bmatrix}^T$ and $\vec{w}=\begin{bmatrix} 0 & 0 & 1 \end{bmatrix}^T$.

<font color='Green'><b>Solution</b></font>: 
We have,
\begin{align*}
\vec{u}\times \vec{v}=\det\left(\begin{bmatrix}\vec{i} & \vec{j} & \vec{k} \\ 1 & 0& 0\\ 0 & 1 & 0\end{bmatrix}\right)=
\begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix}.
\end{align*}

\begin{align*}
\text{the volume of the parallelepiped}&=|(\vec{u}\times \vec{v})\bullet \vec{w}|
=\left|\begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix}\bullet \begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix}\right|=1.
\end{align*}
An alternative way to get the same result:
\begin{align*}
\text{the volume of the parallelepiped}&=
\left|\det\left(\begin{bmatrix}1 & 0 & 0\\ 0 & 1 & 0\\ 0 & 0 & 1 \end{bmatrix}\right)\right|=1.
\end{align*}

***
<font color='Blue'><b>Example</b></font>:
Find the volume of the parallelepiped determined by the vectors $\begin{bmatrix} 1& -7&-5 \end{bmatrix}^T$, $\begin{bmatrix} 1 & -2 & -6 \end{bmatrix}^T$
and $\begin{bmatrix} 3 & 2 &3 \end{bmatrix}^T$.

<font color='Green'><b>Solution</b></font>: 
\begin{align*}
\det\left(\begin{bmatrix} 1 & -7 & -5\\ 1 & -2 & -6\\ 3 & 2 & 3 \end{bmatrix}\right)=
(1)\left|\begin{array}{cc}-2 & -6\\ 2 & 3 \end{array}\right|-(-7)\left|(1)\begin{array}{cc}1 & -6\\ 3 & 3 \end{array}\right|
+(-5)\left|\begin{array}{cc}1 & -2 \\ 3 & 2 \end{array}\right|=113
\end{align*}

\begin{align*}
\text{The volume of the parallelepiped}=\left| 113 \right|=113.
\end{align*}


<div class="alert alert-block alert-success">
<font size="+1"><b>
Lemma:
</b></font>
    
<p>Let <span class="math inline">\(\vec{u}\)</span>, <span class="math inline">\(\vec{v}\)</span>, <span class="math inline">\(\vec{w}\)</span> be three vectors in <span class="math inline">\(\mathbb{R}^n\)</span> that define a parallelepiped. If the volume of the parallelepiped is zero they lie in the same plane and if the volume is not zero they do not lie in the same plane.</p>


    
</div>

<font color='Blue'><b>Example</b></font>:
Determine whether the three vectors $\begin{bmatrix} 1 & 4 & -7 \end{bmatrix}^T$, $\begin{bmatrix} 2 & -1 & 4 \end{bmatrix}^T$ and $\begin{bmatrix} 0 & -9 & 18 \end{bmatrix}^T$   lie in the same plane or not.

<font color='Green'><b>Solution</b></font>: 
\begin{align*}
\text{The volume}&=\left|\det\left(\begin{bmatrix}  1 & 4 & -7\\ 2 & -1 & 4\\ 0 & -9 & 18 \end{bmatrix}\right)\right|=0
\quad \Rightarrow\quad \text{The three points lie in the same plane.}
\end{align*}

<center>
<iframe src="https://www.geogebra.org/classic/eb8s7rza?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>
</center>

***

<font color='Blue'><b>Example</b></font>:
Given lines
$L_1:~\begin{bmatrix} x\\y\\z \end{bmatrix}=\begin{bmatrix} 2\\ 1\\ -1 \end{bmatrix}+s\begin{bmatrix} 1\\ 1\\ -1 \end{bmatrix}$
and
$L_2:~\begin{bmatrix} x\\y\\z \end{bmatrix}=\begin{bmatrix} 1\\ 2\\ 0 \end{bmatrix}+t\begin{bmatrix} 1\\ 1\\ 1 \end{bmatrix}$,  find the shortest distance between them and points $P_1$ on $L_1$ and $P_2$ on $L_2$ that are closest.

<font color='Green'><b>Solution</b></font>: 
```{image} ../Figures/fig4_32.png
:width: 180px
:align: center
```

Let $P_1=(2,1,-1)$ on $L_1$ and $P_2=(1,2,0)$ on $L_2$. It follows that $\overrightarrow{P_1P_2}=\begin{bmatrix} -1 & 1 & 1 \end{bmatrix}^T$. Moreover, the direction of the $L_1$ and $L_2$ are $\vec{d}_1=\begin{bmatrix} 1 & 1 & -1 \end{bmatrix}^T$ and $\vec{d}_2=\begin{bmatrix} 1 & 1 & 1 \end{bmatrix}^T$,  respectively.

The two lines are not parallel since
\begin{align*}
\vec{d_1}\times \vec{d_2}&=\left|\begin{array}{ccc} \vec{i} & \vec{j} & \vec{k}\\ 1 & 1 & -1\\ 1 & 1 & 1\\ \end{array}\right|
=\left[\begin{array}{c} 2\\ -2\\ 0 \end{array}\right]\neq\left[\begin{array}{c} 0\\ 0\\ 0 \end{array}\right].
\end{align*}
Furthermore, let $\vec{n}= \vec{d_1}\times \vec{d_2}=\begin{bmatrix} 2 & -2 & 0 \end{bmatrix}^T$ and
\begin{align*}
proj_{\vec{n}}\overrightarrow{P_1P_2}&=\frac{\overrightarrow{P_1P_2}\bullet \vec{n}}{\vec{n}\bullet \vec{n}}\vec{n}
=\frac{\begin{bmatrix} -1\\ 1\\ 1\end{bmatrix}\bullet \begin{bmatrix}2\\ -2\\ 0\end{bmatrix}}{\begin{bmatrix}2\\ -2\\ 0\end{bmatrix}\bullet \begin{bmatrix}2\\ -2\\ 0\end{bmatrix}}\begin{bmatrix}2\\ -2\\ 0\end{bmatrix}
=\frac{-4}{8}\begin{bmatrix}2\\ -2\\ 0\end{bmatrix}
=\begin{bmatrix}-1\\ 1\\ 0\end{bmatrix}
\end{align*}
Therefore,
\begin{align*}
\text{The shortest distance}=\|proj_{\vec{n}}\overrightarrow{P_1P_2}\|=\sqrt{1+1}=\sqrt{2}.
\end{align*}

***
<font color='Blue'><b>Example</b></font>:
Find the shortest distance between the following two lines in $\mathbb{R}^3$
$$
L_1:
\begin{cases}
x=t+2\\ y=t\\z= t-1
\end{cases}
\quad
L_2:
\begin{cases}
x=2\,s+2\\ y=2\,s\\z= 2\,s+2
\end{cases}
$$

<font color='Green'><b>Solution</b></font>: 
```{image} ../Figures/fig4_39.png
:width: 250px
:align: center
```

Let $P_1=(2,0,-1)$ on $L_1$ and $P_2=(2,0,2)$ on $L_2$. Therefore, $\overrightarrow{P_1P_2}=\begin{bmatrix}0 & 0 & 3\end{bmatrix}^T$. Moreover, the directions of the $L_1$ and $L_2$ are $\vec{d}_1=\begin{bmatrix}1 & 1 & 1 \end{bmatrix}^T$ and
 $\vec{d}_2=\begin{bmatrix} 2 & 2 & 2 \end{bmatrix}^T$,  respectively.

Note that the two lines are parallel since
\begin{align*}
\vec{d_1}\times \vec{d_2}&=\left|\begin{array}{ccc} \vec{i} & \vec{j} & \vec{k}\\ 1 & 1 & 1\\ 2 & 2 & 2 \\ \end{array}\right|
=\left[\begin{array}{c} 0\\ 0\\ 0 \end{array}\right].
\end{align*}
Therefore,
\begin{align*}
\overrightarrow{0Q}&=\overrightarrow{0P_1}+ \overrightarrow{P_1Q}= \overrightarrow{0P_1}+ proj_{\vec{d_1}}{\overrightarrow{P_1P_2}}
\\ &
= \begin{bmatrix} 2\\ 0\\ -1 \end{bmatrix}+
\frac{\begin{bmatrix} 0\\ 0\\ 3\end{bmatrix}\bullet \begin{bmatrix}1\\ 1\\ 1\end{bmatrix}}{\begin{bmatrix}1\\ 1\\ 1\end{bmatrix}\bullet
 \begin{bmatrix}1\\ 1\\ 1\end{bmatrix}}\begin{bmatrix}1\\ 1\\ 1\end{bmatrix}
\\&
=\begin{bmatrix} 2\\ 0\\ -1 \end{bmatrix}+\begin{bmatrix}1\\ 1\\ 1\end{bmatrix}=\begin{bmatrix} 3\\ 1\\ 0 \end{bmatrix}
\end{align*}
$Q$ is a point on $L_1$ (why!?). Therefore, the shortest distance is the length of $\overrightarrow{QP_2}$ (or $\overrightarrow{P_2Q}$)
\begin{align*}
\overrightarrow{QP_2}=\begin{bmatrix} 2\\ 0\\ 2 \end{bmatrix}-\begin{bmatrix} 3\\ 1\\ 0 \end{bmatrix}=\begin{bmatrix} -1\\ -1\\ 2\end{bmatrix}.
\end{align*}
and
\begin{align*}
\text{The shortest distance}=\|\overrightarrow{QP_2}\|=\sqrt{6}.
\end{align*}

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
***
