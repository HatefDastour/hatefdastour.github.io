# Complex Numbers

Complex numbers have two components real part and the imaginary part. A complex number is usually expressed as $z = a+b\,i$, where $a$ and $b$ are real numbers, and $i$ is a symbol for indicating the imaginary part ($i^2=-1$). The real part of the complex number $z = a+b\,i$ is the real number $a$, and the imaginary part is the real number $b$.


A Complex number can be expressed by the ordered pair. This representation can be convenient in plotting this number in the Argand plane. However, here the horizontal axis is called the **real axis**, and the vertical axis is called the **imaginary axis**.

<center>
<iframe src="https://www.desmos.com/calculator/zvu0kgtj3y?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>
</center>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
The field of real numbers denoted as $\mathbb{R}$ and the field of complex numbers denoted $\mathbb{C}$.
</div>

## Addition and Subtraction of Complex Numbers

Complex numbers $z_1=a+bi$ and $z_2=c+di$, are equal only if their real parts are equal, and their imaginary parts are equal. That is
\begin{align*}
a=c \quad \text{and} \quad b=d
\end{align*}

Now, for two complex numbers $z_1=a+bi$ and $z_2=c+di$, we have

* **Addition**: $z_1+z_2=\left(a+b\,i\right)+\left(c+d\,i\right)=\left(a+c\right)+\left(b+d\right)\,i,$
* **Subtraction**: $z_1-z_2=\left(a+b\,i\right)-\left(c+d\,i\right)=\left(a-c\right)+\left(b-d\right)\,i.$

<font color='Blue'><b>Example</b></font>:
-   $(-3+6i) + (5-i) =  2+5i$.

-   $(4-7i) + (6-2i) =  10-9i$.

-   $(-3+6i) - (5-i) =  -8+7i$.

-   $(4-7i) - (6-2i) =  -2-5i$.

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Proposition: Properties of Addition
</b></font>
    
* $z + w = w + z$. <font color='Blue'>(addition is commutative)</font>

* $(z + w) + v = z + (w + v)$. <font color='Blue'>(addition is associative)</font>

* $z + 0 =0+z= z$. <font color='Blue'>(existence of an additive identity)</font>

* For every $z=a+bi$ there exists a complex number $-z = -a -bi$ such that
\\$z + (-z) =(-z)+z=0.$ <font color='Blue'>(existence of an additive inverse)</font>
</div>

If $z=a+bi$ and $w=c+di$, then $z+w=(a+c)+(b+d)i$.

Geometrically, we have:
```{image} ../Figures/fig6_00.png
:width: 320px
:align: center
```

We can see that $0$, $z$, $w$, and $z+w$ are the vertices of a parallelogram.

## Multiplication of Complex Numbers

The product of complex numbers two complex numbers $z_1=a+b\,i$ and $z_2=c+d\,i$, we have,
\begin{align*}
z_1z_2=\left(a+b\,i\right)\left(c+d\,i\right)=a\left(c+d\,i\right)+b\,i\left(c+d\,i\right)=
ac+ad\,i+bc\,i+bd\,i^2.
\end{align*}
Since $i^2=-1$, this becomes
\begin{align*}
\left(a+b\,i\right)\left(c+d\,i\right)=ac+ad\,i+bc\,i-bd=\left(ac-bd\right)+\left(ad+bc\right)\,i.
\end{align*}

<font color='Blue'><b>Example</b></font>: Multiplication of Complex Numbers

\begin{align*}
(2-3i)(-3+4i) &= ((2)(-3) - (-3)(4))+((2)(4)+(-3)(-3))i \\
&= (-6 + 12) + (8 + 9)i = 6+17i
\end{align*}
Similarly,
\begin{align*}
\left(2+\,i\right)\left(2+3\,i\right)&=1+8\,i,\\
\left(1+i\right)\left(1-i\right)&=2,\\
\left(2+i\right)\left(1+2\,i\right)&=5\,i.
\end{align*}

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: Properties of Multiplication of Complex Numbers
</b></font>
    
<p>Let <span class="math inline">\(z, w\)</span> and <span class="math inline">\(v\)</span> be complex numbers.</p>
<ul>
<li><p><span class="math inline">\(zw=wz\)</span>.</p></li>
<li><p><span class="math inline">\((zw)v=z(wv)\)</span>.</p></li>
<li><p><span class="math inline">\(z (w+v) = zw + zv\)</span>.</p></li>
<li><p><span class="math inline">\(1z=z\)</span>.</p></li>
<li><p>For each <span class="math inline">\(z \neq 0\)</span>, there exists <span class="math inline">\(z^{-1}\)</span> such that<br />
<span class="math inline">\(z z^{-1} =z^{-1}z= 1\)</span>.</p></li>
</ul>
    
</div>

<font color='Blue'><b>Example</b></font>:
Find all complex numbers $z=a+bi$ with $b\neq 0$ such that $z^2=-3+4i$.

<font color='Green'><b>Solution</b></font>: 
We have
\begin{align*}
z^2=(a+bi)^2=(a^2-b^2)+2abi = -3+4i,
\end{align*}
Hence,
\begin{align*}
a^2-b^2=-3 \mbox{ and } 2ab=4.
\end{align*}
Since $2ab=4$, $a=\frac{2}{b}$.

Substituting this into the first equation gives us

\begin{eqnarray*}
a^2-b^2 & = & -3 \\
\left(\frac{2}{b}\right)^2 - b^2 & = & -3 \\
\frac{4}{b^2} - b^2 & = & -3 \\
4- b^4 & = & -3b^2 \\
b^4-3b^2-4 & = & 0.
\end{eqnarray*}
Now, $b^4-3b^2-4=0$ can be factored  into
\begin{eqnarray*}
(b^2-4)(b^2+1)& = & 0\\
(b-2)(b+2)(b^2+1)& = & 0.
\end{eqnarray*}
Since $b\in \mathbb{R}$ and $b^2+1$ has no real roots, $b=2$ or $b=-2$.

Since $a=\frac{2}{b}$, it follows that

-   when $b=2$, $a=1$, and $z=a+bi=1+2i$;

-   when $b=-2$, $a=-1$, and $z=a+bi=-1-2i$.

Therefore, if $z^2=-3+4i$, then $z=1+2i$ or $z=-1-2i$.

## The Conjugate of a Complex Number

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Conjugate of a Complex Number
</b></font>

For the complex number $z = a+b\,i$, we define its \textbf{complex conjugate} to be $\overline{z} = a-b\,i$.
$$\overline{z} = \overline{a+b\,i}=a-b\,i.$$

<font color='Blue'><b>Example</b></font>:
Conjugate of a Complex Number
</b></font>

\begin{align*}
\overline{2+\,i}&=2-\,i,\\
\overline{i}&=-i,\\
\overline{1}&=1.
\end{align*}
</div>

The geometric interpretation of the complex conjugate is shown in Figure following figure.

<center>
<iframe src="https://www.geogebra.org/classic/uxsbnzbk?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>
</center>

Some of the properties of the complex conjugate are listed in the following theorem.

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Properties of the Conjugate
</b></font>
    
Let $z$ and $w$ be complex numbers. Then, the following properties of the conjugate hold.

* $\overline{z\pm w}=\overline{z}\pm \overline{w}$,
* $\overline{zw} = \overline{z}\, \overline{w}$,
* $\overline{\left(\overline{z}\right)} = z$,
* $\overline{\left(\dfrac{z}{w}\right)}=\dfrac{\overline{z}}{\overline{w}}$,
* $z$ is real if and only if $\overline{z} = z$.
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
Let $z=a+b\,i$ be a complex number. Then,
\begin{align*}
z\overline{z}=\left(a+b\,i\right)\left(a-b\,i\right)=\left(a^2+b^2\right)+\left(ab-ab\right)\,i=a^2+b^2.
\end{align*}
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
The quotient $z=a+b\,i$ divided by $w=c+d\,i$, where $c^2+d^2\neq0$, is
\begin{align*}
\dfrac{z}{w}&=\dfrac{a+b\,i}{c+d\,i}=\dfrac{\left(a+b\,i\right)}{\left(c+d\,i\right)}\times\dfrac{\left(c-d\,i\right)}{\left(c-d\,i\right)}=
\dfrac{\left(a+b\,i\right)\left(c-d\,i\right)}{\left(c+d\,i\right)\left(c-d\,i\right)}=
\dfrac{\left(a+b\,i\right)\left(c-d\,i\right)}{c^2+d^2}
\\ &
=\dfrac{1}{c^2+d^2}\left(a+b\,i\right)\left(c-d\,i\right)=
\left(\dfrac{ac+bd}{c^2+d^2}\right)+\left(\dfrac{bc-ad}{c^2+d^2}\right)\,i
\end{align*}
</div>

<font color='Blue'><b>Example</b></font>:
\begin{align*}
\begin{array}{ll}
\bullet &
\dfrac{1}{i} =  \dfrac{1}{i}\times \dfrac{-i}{-i}=\dfrac{-i}{-i^2}=-i.
\\\\
\bullet &
\dfrac{2-i}{3+4i} =  \dfrac{2-i}{3+4i}\times \dfrac{3-4i}{3-4i}=\dfrac{(6-4)+(-3-8)i}{3^2+4^2}=\dfrac{2-11i}{25}=\dfrac{2}{25} - \dfrac{11}{25}i.
\\\\
\bullet &
\dfrac{1-2i}{-2+5i} =  \dfrac{1-2i}{-2+5i}\times \dfrac{-2-5i}{-2-5i}=\dfrac{(-2-10) + (4-5)i}{2^2+5^2}=-\dfrac{12}{29}-\dfrac{1}{29}i.
\end{array}
\end{align*}

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Inverse of a Complex Number
</b></font>

Let $z=a+b\,i$ be a complex number. Then the multiplicative inverse of $z$, written $z^{-1}$ exists if and only if $a^2 +b^2 \neq 0$ and is given by
\begin{align*}
z^{-1}&=\frac{1}{a+b\,i}=\frac{1}{\left(a+b\,i\right)}\times\frac{\left(a-b\,i\right)}{\left(a-b\,i\right)}
=\frac{\left(a-b\,i\right)}{\left(a+b\,i\right)\left(a-b\,i\right)}=\frac{1}{a^2+b^2}\left(a-b\,i\right)
\\ &
=\frac{a}{a^2+b^2}-\frac{b}{a^2+b^2}i.
\end{align*}
</div>

<font color='Blue'><b>Example</b></font>:
When $z = 2 + 6i$, $z^{-1}$ is defined, and

\begin{align*}
\frac{1}{z}=\frac{1}{2+6i} =\frac{1}{2+6i}\times \frac{2-6i}{2-6i}=\frac{2-6i}{2^2+6^2} =
\frac{2-6i}{40} =
\frac{1}{20} -  \frac{3}{20}i.
\end{align*}

Note that we can always check that $zz^{-1}=1$.

## The Absolute Value (Modulus) of a Complex Number

**Absolute Value**: The **modulus**, or **absolute value,** of a complex number$z=a+b\,i$ is
its distance from the origin.
\begin{align*}
|z|=|a+b\,i| = \sqrt{a^2+b^2}.
\end{align*}

<center>
<iframe src="https://www.geogebra.org/classic/uxsbnzbk?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>
</center>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Properties of the Modulus
</b></font>
    
* $z\overline{z}=\left(a+b\,i\right)\left(a-b\,i\right)=a^2+ab\,i-ab\,i-b\,i^2=a^2+b^2=|z|^2$.
* $\dfrac{1}{z}= \dfrac{\overline{z}}{|z|^2}$.
* $|z|\geq 0$ for all $z$.
* $|z|=0$ if and only if $z=0$.
* $\dfrac{z}{w}=\dfrac{z}{w}\dfrac{\overline{w}}{\overline{w}}=\dfrac{z\overline{w}}{|w|^2}.$  
</div>

<font color='Blue'><b>Example</b></font>:
1.  $|-3+4i|=\sqrt{3^2+4^2}= \sqrt{25}= 5$.

2.  $|3-2i|= \sqrt{3^2+2^2}=\sqrt{13}$.

3.  $|i|= \sqrt{1^2}=1$.

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem:
</b></font>
    
* For complex numbers $z=a+b\,i$ and $w=c+d\,i$,
$$|zw|=|z||w|.$$
* For complex numbers $z=a+b\,i$ and $w=c+d\,i$ such that $c^2+d^2\neq0$
$$\left|\frac{z}{w}\right|=\frac{|z|}{|w|}.$$
* For complex numbers $z=a+b\,i$ and $c\in \mathbb{R}$,
$$|cz|=|c||z|.$$
</div>

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Triangle Inequality
</b></font>
    
<p>Let <span class="math inline">\(z\)</span>, <span class="math inline">\(w\)</span> be complex numbers. The following two inequalities hold for any complex numbers <span class="math inline">\(z\)</span>, <span class="math inline">\(w\)</span>: <span class="math display">\[\begin{aligned}
|z+w| \leq |z|+|w|,\\
\left||z|-|w|\right| \leq |z-w|\end{aligned}\]</span> The first one is called the Triangle Inequality.</p>
    
</div>

<font color='Blue'><b>Example</b></font>:
Let $z=4-3i$, $w=1+i$, and $u=2-2i$. Then,
$\left|\dfrac{w-\overline{wu}}{zu}\right|$ equals

a) $\dfrac{1}{10\sqrt{2}}$

b) $\dfrac{1}{2\sqrt{5}}$

c) $\dfrac{1}{5}$

d) $\dfrac{9}{10\sqrt{2}}$

e) $\dfrac{1}{\sqrt{2}}$

<font color='Green'><b>Solution</b></font>: 
We are going to use the following fact,

<div class="alert alert-block alert-success">
<p><span class="math display">\[\left| c(a+bi)\right|=|c||a+bi|=|c|\sqrt{a^2+b^2}.\]</span></p>

</div>

\begin{align*}
\dfrac{w-\overline{wu}}{zu}&=\dfrac{(1+i)-\overline{(1+i)(2-2i)}}{(4-3i)(2-2i)}=
\dfrac{(1+i)-\overline{4}}{2-14i}=\dfrac{(1+i)-4}{2-14i}=\dfrac{-3+i}{2-14i}
\\ &
=\dfrac{(-3+i)}{(2-14i)}\dfrac{(2+14i)}{(2+14i)}=\dfrac{1}{10\,\sqrt{2}}\left(-20-40i\right)
=-\frac{1}{10}-\frac{1}{5}i=-\frac{1}{10}\left(1+2i\right).
\end{align*}
Therefore,
\begin{align*}
\left|\dfrac{w-\overline{wu}}{zu}\right|=\frac{\sqrt{5}}{10}=\frac{\sqrt{5}}{10}\frac{\sqrt{5}}{5}=
\frac{5}{10\sqrt{5}}=\frac{1}{2\sqrt{5}}.
\end{align*}

***
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
1. Stewart, James, Daniel K. Clegg, and Saleem Watson. Calculus: early transcendentals. Cengage Learning, 2020.
***
