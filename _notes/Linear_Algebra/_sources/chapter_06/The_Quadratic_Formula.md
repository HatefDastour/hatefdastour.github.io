
The Quadratic Formula
========================

Since $i^2=-1$, we can think of as a square root of $-1$. But notice
that we also have $(-i)^2=i^2=-1$ and so $-i$ is also a square root of
$-1$. We say that is the **principal square root** of $-1$ and write
$\sqrt{-1}=i$. In general, if $c$ is any positive number, we write
\begin{align*}
\sqrt{-c}=\sqrt{c}i
\end{align*}
With this convention, the usual
derivation and formula for the roots of the quadratic equation
$ax^2+bx+c=0$ are valid even when $b^2-4ac<0$,
\begin{align*}
x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}
=\left\{ \begin{array}{l}
\dfrac{-b+\sqrt{b^2-4ac}}{2a}
\\
\dfrac{-b-\sqrt{b^2-4ac}}{2a}
\end{array}\right.
\end{align*}

-   if $b^2-4ac\geq 0$, then the roots of the quadratic are **real**;

-   if $b^2-4ac<0$, then the quadratic has **no real roots**.

<font color='Blue'><b>Example</b></font>:
Find the roots of the equation $x^2+x+1=0$.

<font color='Green'><b>Solution</b></font>: 
Using the quadratic formula, we have
\begin{align*}
x=\frac{-1\pm\sqrt{1^2-4(1)(1)}}{2(1)}=\frac{-1\pm\sqrt{1-4}}{2}=\frac{-1\pm\sqrt{3}i}{2}
=\begin{cases}
\dfrac{-1+\sqrt{3}i}{2}
\\
\dfrac{-1-\sqrt{3}i}{2}
\end{cases}
=\begin{cases}
-\dfrac{1}{2}-\dfrac{\sqrt{3}\,i}{2}
\\
 -\dfrac{1}{2}+\dfrac{\sqrt{3}\,i}{2}
\end{cases}
\end{align*}

<div class="alert alert-block alert-info">
<font size="+1"><b>
Theorem: The Fundamental Theorem of Algebra
</b></font>
    
<p>Every polynomial of positive degree with complex coefficients has a complex root.</p>


</div>

<font color='Blue'><b>Example</b></font>:
Find the roots of the quadratic $x^2-(3-2i)x+(5-i)=0$.

<font color='Green'><b>Solution</b></font>: 
Using the quadratic formula
\begin{align*}
x=\frac{(3-2i) \pm\sqrt{(-(3-2i))^2-4(5-i)}}{2}.
\end{align*}
Note that
\begin{align*}  (-(3-2i))^2-4(5-i) = 5-12i-20+4i=-15-8i,\end{align*}
Hence,
\begin{align*} x=\frac{3-2i \pm\sqrt{-15-8i}}{2}.\end{align*}

To find $\pm\sqrt{-15-8i}$, solve $z^2=-15-8i$ for $z$.
Let $z=a+bi$ and $z^2=-15-8i$.

Then
\begin{align*} &(a^2-b^2)+2abi=-15-8i,
\quad \Rightarrow \quad
\begin{cases}
a^2-b^2=-15,
\\
2ab=-8.
\end{cases}
\quad \Rightarrow \quad
\begin{cases}
a^2-b^2=-15,
\\
a=-4/b.
\end{cases}
\end{align*}
Solving for $a$ and $b$
\begin{align*}
\left(-\frac{4}{b}\right)^2-b^2=-15
\quad \Rightarrow \quad
(b-4) (b+4) \underbrace{(b^2+1)}_{\text{No real roots!}}=0
\quad \Rightarrow \quad
b=\pm 4\\
\text{Since }a=-4/b \Rightarrow \quad a=\mp 1.
\end{align*}
Therefore, $z= 1-4i, -1+4i$, i.e., $z=\pm(1-4i)$. We have,
\begin{align*}
x=\frac{(3-2i) \pm(1-4i)}{2}=
\begin{cases}
\dfrac{(3-2i) +(1-4i)}{2}
=\dfrac{4-6i}{2} = 2-3i,
\\
\dfrac{(3-2i) -(1-4i)}{2}
=\dfrac{2+2i}{2}= 1+i.
\end{cases}\end{align*}

Thus, the roots of $x^2-(3-2i)x+(5-i)$ are $2-3i$ and $1+i$.

***
## Refrences
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
1. Stewart, James, Daniel K. Clegg, and Saleem Watson. Calculus: early transcendentals. Cengage Learning, 2020.
***
