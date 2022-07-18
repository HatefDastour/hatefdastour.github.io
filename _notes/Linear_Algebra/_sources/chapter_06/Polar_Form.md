# Polar Form

Let $z=a+bi$ be a complex number and $r$ denote the distance $z$ from the origin, i.e. $r=|z|=\sqrt{a^2+b^2}$. Also, let $\theta$ represent the angle between the line through $0$ and $z$ and the positive $x$-axis (this angle is measured clockwise direction). See the following figure. Then, $\theta$ is defined by $\cos\theta = \dfrac{a}{r}$ and $\sin\theta=\dfrac{b}{r}$. This angle $\theta$ is called the argument of $z$, and it is shown by $\arg z=\theta$.

<center>
<iframe src="https://www.geogebra.org/classic/jqkh34yt?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>
</center>

## Euler's formula

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Euler's formula
</b></font>

\begin{align*}
e^{i\theta}=\cos(\theta)+i\,\sin(\theta)
\end{align*}

</div>

The polar form of the complex number $z = a+b\,i = r(\cos(\theta) +i\sin(\theta) )$ can be also written as follows,
\begin{align*} z =re^{i\theta} \end{align*}
where $\theta$ is the argument of $z$.

<font color='Blue'><b>Example</b></font>:
Find the polar form for the number $z=1$.

<font color='Green'><b>Solution</b></font>: 
To convert $z$ to polar form, we need to find $r$ and $\theta$ so that $1=re^{i\theta}$.

Now $r=|z|=\sqrt{1^2}=1$, and $\theta=0$ is an argument for $z=1$. However, we may also write
\begin{align*}
1=e^{2\pi i}, 1=e^{-2\pi i}, e^{4\pi i}, e^{6\pi i}, \ldots
\end{align*}
Since sine and cosine have periodicity $2\pi$, we may add (or subtract) multiples of $2\pi$ to any argument.

## Principal Argument
Angle $\theta$ is known as the argument of $z$ (denoted by $\arg(z)$). This angle is not unique as 
\begin{align*}
\theta = \theta  + 2\pi = \theta + 4\pi = \ldots = \theta + 2k\pi,~k\in \mathbb{N}
\end{align*}
The principal argument of $z$, on the other hand, is the unique angle $\theta \in (- \pi , \pi]$ such that
\begin{align*}
\begin{cases}
\cos(\theta)=\dfrac{a}{r},\\
\sin(\theta)=\dfrac{b}{r}.
\end{cases}
\end{align*}

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Principal Argument
</b></font>

For a complex number $z$ with $|z|=r$, the \textbf{principal argument} of $z$ is the unique angle $\theta=\arg (z)$ (measured in radians) such that
\begin{align*}
-\pi < \theta \leq \pi.
\end{align*}
</div>

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Polar Form of a Complex Number
</b></font>

Let $z = a+b\,i$ be a complex number. Then the polar form of $z$ is written as
\begin{align*}z = re^{i\theta}\end{align*}
where $r = \sqrt{a^2+b^2}$ and $\theta$ is the (principal) argument of $z$.
</div>

<center>
<iframe src="https://www.geogebra.org/classic/wdrrje5w?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>
</center>

<font color='Blue'><b>Example</b></font>:
Convert the number $z = -2 +2\sqrt{3}i$ to polar form.

<font color='Green'><b>Solution</b></font>: 
To convert $z$ to polar form,
we need to find $r$ and $\theta$ so that
$-2+2\sqrt{3}i=re^{i\theta}$.

Since $r=|z|$,
\begin{align*}
r=\sqrt{(-2)^2 + (2\sqrt{3})^2}
 = \sqrt{4+4(3)}
 = \sqrt{16}  = 4
\end{align*}

There are two approaches to finding an argument, $\theta$. The first approach to plot $-2+2\sqrt{3}$ in the complex plane.

<center>
<iframe src="https://www.geogebra.org/classic/bpj9qvay?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>
</center>

<center>

|    $\theta$    | $0$ |    $\frac{\pi}{6}$   |    $\frac{\pi}{4}$   |    $\frac{\pi}{3}$   | $\frac{\pi}{2}$ |   $\frac{2\pi}{3}$   |    $\frac{3\pi}{4}$   |    $\frac{5\pi}{6}$   | $\pi$ | $\frac{3\pi}{2}$ | $2\pi$ |
|:--------------:|:---:|:--------------------:|:--------------------:|:--------------------:|:---------------:|:--------------------:|:---------------------:|:---------------------:|:-----:|:----------------:|:------:|
| $\sin(\theta)$ | $0$ |     $\frac{1}{2}$    | $\frac{\sqrt{2}}{2}$ | $\frac{\sqrt{3}}{2}$ |       $1$       | $\frac{\sqrt{3}}{2}$ |  $\frac{\sqrt{2}}{2}$ |     $\frac{1}{2}$     |  $0$  |       $-1$       |   $0$  |
| $\cos(\theta)$ | $1$ | $\frac{\sqrt{3}}{2}$ | $\frac{\sqrt{2}}{2}$ |     $\frac{1}{2}$    |       $0$       |    $-\frac{1}{2}$    | $-\frac{\sqrt{2}}{2}$ | $-\frac{\sqrt{3}}{2}$ |  $-1$ |        $0$       |   $1$  |

</center>

From the above table, it can be seen that $\theta = \frac{2\pi}{3}$, and $z$ can be written in polar form as $z=4e^{i(2\pi/3)}$.
***

<font color='Blue'><b>Example</b></font>:

a.  Let $z = -\dfrac{1}{2}+\dfrac{\sqrt{3}}{2}i$ be a complex number.
    Write $z$ in the polar form $z =re^{i\theta}$.

b.  Let $z = 2\,e^{i\pi/6}$. Write $z$ in the standard (Cartesian) form
    $z = a+b\,i$.

<font color='Green'><b>Solution</b></font>:

a.  We have
$r=|z|=\sqrt{\left(-\frac{1}{2}\right)^2+\left(\frac{\sqrt{3}}{2}\right)^2}=\sqrt{\frac{1}{4}+\frac{3}{4}}=1$,
and
\begin{align*}
a=-\frac{1}{2}, b=\frac{\sqrt{3}}{2}\Rightarrow \quad
\begin{cases}
\cos(\theta)=-\frac{1}{2},\\
\sin(\theta)=\frac{\sqrt{3}}{2}.
\end{cases}
\end{align*}
We know that
$\theta \in (- \pi , \pi]$;
therefore,
$\theta=\frac{2\pi}{3}$, and $z = e^{i\,2\pi/3}$.


<center>
<iframe src="https://www.geogebra.org/classic/e7rvst7c?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>
</center>

b.  We have
\begin{align*}
r=2, \theta=\frac{\pi}{6} \Rightarrow \quad
\begin{cases}
a=2\,\cos\left(\frac{\pi}{6}\right)=\sqrt{3},\\
b=2\,\sin\left(\frac{\pi}{6}\right)=1.
\end{cases}\end{align*}
Therefore, $z=\sqrt{3}+i$.

Note that you could directly write down the answer as
\begin{align*}
a+b\,i&=\left(r\,\cos(\theta)\right)+\left(r\,\sin(\theta)\right)i=r\left(\cos(\theta)+i\,\sin(\theta)\right)
\\&
=2\,\left(\cos\left(\frac{\pi}{6}\right)+i\sin\left(\frac{\pi}{6}\right)\right)=
\sqrt{3}+i.
\end{align*}

***
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
1. Stewart, James, Daniel K. Clegg, and Saleem Watson. Calculus: early transcendentals. Cengage Learning, 2020.
***