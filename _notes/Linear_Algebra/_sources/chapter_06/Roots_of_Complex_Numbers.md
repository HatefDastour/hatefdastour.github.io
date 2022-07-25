# Roots of Complex Numbers



<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: De Moivre’s Theorem
</b></font>
    
If $z=re^{i\theta}$ and $n$ is a positive integer,
\begin{align*}\left(re^{i\theta}\right)^n=r^n e^{i\,n\theta}= r^n\left(\cos(n\theta) +i\sin(n\theta)\right).\end{align*}
or
\begin{align*}\left(r\left(\cos(\theta) +i\sin(\theta)\right)\right)^n=r^n\left(\cos(n\theta) +i\sin(n\theta)\right).\end{align*}
</div>

Using this theorem, instead of taking the $n^{\text{th}}$ power of a complex number, we can simply multiply the argument by $n$.

<font color='Blue'><b>Example</b></font>:
1.  Find $z^{10}=\left(\dfrac{1}{2}+\dfrac{1}{2}i\right)^{10}$.

2.  If $w = 2\,e^{i\pi/6}$, find $w^{-1}$.

<font color='Green'><b>Solution</b></font>: 
1.  Firstly, we need to write down $z$ in $e^{i\theta}$ form. It can be
    seen that
	\begin{align*}
    r=|z|=\sqrt{\frac{1}{4}+\frac{1}{4}}=\frac{\sqrt{2}}{{2}}=\frac{1}{\sqrt{2}}\quad \text{and}\quad
    \begin{cases}
    \cos(\theta)=\dfrac{1/2}{\sqrt{2}/2}=\dfrac{\sqrt{2}}{2},\\
    \sin(\theta)=\dfrac{1/2}{\sqrt{2}/2}=\dfrac{\sqrt{2}}{2}.
    \end{cases}
	\end{align*}
    As the the principal argument
	$\theta \in (- \pi , \pi]$, $\theta=\frac{\pi}{4}$.
    
    Therefore,
	\begin{align*}
    z^{10}&=\left(\dfrac{1}{2}+\dfrac{1}{2}i\right)^{10}=\left(\frac{1}{\sqrt{2}}e^{\frac{\pi}{4}i} \right)^{10}
    =\left(\frac{1}{\sqrt{2}}\right)^{10} \left(\cos\left(10\frac{\pi}{4}\right) +i\sin\left(10\frac{\pi}{4}\right)\right)
    \\ &
    =\left(\frac{1}{(2)^{5}}\right) \left(\cos\left(\frac{5\pi}{2}\right) +i\sin\left(\frac{5\pi}{2}\right)\right)
    =\left(\frac{1}{32}\right) \left(\cos\left(\frac{\pi}{2}\right) +i\sin\left(\frac{\pi}{2}\right)\right)
    \\ &
    =\left(\frac{1}{32}\right) \left(0 +i\right)=\frac{i}{32}.
	\end{align*}
    Note that $\dfrac{5\pi}{2}=2\pi+\dfrac{\pi}{2}$ and
    $\begin{cases}\cos(5\pi/2)=\cos(\pi/2),\\ \sin(5\pi/2)=\sin(\pi/2).\end{cases}$.

2.  
	\begin{align*}
    w^{-1}&=\left(2\,e^{i\pi/6}\right)^{-1}=2^{-1}\,e^{-i\pi/6}
    \\ &
    =\frac{1}{2}\,e^{-i\pi/6}=\frac{1}{2}\left(\cos\left(-\frac{\pi}{6}\right) +i\sin\left(-\frac{\pi}{6}\right)\right)
    \\ &
    =\frac{1}{2}\left(\frac{\sqrt{3}}{2} -\frac{1}{2}\,i\right)=\frac{1}{4}\left(\sqrt{3} -i\right)
    =\frac{\sqrt{3}}{4}-\frac{1}{4}{}i.
	\end{align*}

<div class="alert alert-secondary" role="alert">
<font size="+1"><b>
Theorem: Multiplication Rule
</b></font>
    
For two complex numbers $z_1 = r_1 e^{i\theta_1}$ and $z_2 = r_2 e^{i\theta_2}$ in polar form, we have
\begin{align*}
z_1 z_2 = r_1 r_2 e^{i(\theta_1+\theta_2)}.
\end{align*}
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
Note that for a real number $c\in \mathbb{R}$,
* $c^{0}=1$,
* $c^{1/n}=\sqrt[n]{c}$ for $n=1,2,3,\ldots$,
* If $c\neq 0$, $c^{-n}=\dfrac{1}{c^n}$ for $n=1,2,3,\ldots$.
</div>

<font color='Blue'><b>Example</b></font>:
Express $(1-i)^6(\sqrt{3}+i)^3$ in the form $a+bi$.

<font color='Green'><b>Solution</b></font>: 
Let $z=1-i=\sqrt{2}e^{-\pi i/4}$ and $w=\sqrt{3}+i=2e^{i\pi /6}$.
We want to compute $z^6w^3$.
\begin{eqnarray*}
z^6w^3 & = & (\sqrt{2}e^{-i\pi /4})^6(2e^{i\pi /6})^3 \\
& = & (2^3 e^{-i(6\pi /4)}) (2^3 e^{i(3\pi /6)}) \\
& = & (8 e^{-i(3\pi /2)}) (8 e^{i\pi /2}) \\
& = & 64 e^{-i\pi }\\
& = & 64(\cos(-\pi) + i\sin(-\pi)) \\
& = & 64(\cos(\pi)+0) \\
& = & -64.
\end{eqnarray*}

<div class="alert alert-info" role="alert">
<font size="+1"><b>
Theorem: <span class="math inline">\(n^{th}\)</span> root of <span class="math inline">\(q\)</span>
</b></font>

Complex number $z$ is called \textbf{an $n^{th}$ root of $q$} if $z^n=q$ for some $n\in\mathbb{N}$.
</div>


<font color='Blue'><b>Example</b></font>:

-   $25$ has two square roots, $5$ and $-5$, and these are the two solutions to $z^2=25$.
-   $-1$ has no real square roots, but it has two complex square roots, $i$ and $-i$. These are the two (complex) solutions to $z^2=-1$.
-   $-4$ has two square roots, $2i$ and $-2i$, and these are the two solutions to $z^2=25$.

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Corollary:
</b></font>
    
For a nonzero complex number $q$, $z^n=q$ has exactly $n$ different complex $n^{th}$ roots.   
</div>

It follows from Moivre’s theorem that, for a complex number $z = a+b\,i$ with polar form $z=|z|\left(\cos(\theta) +i\sin(\theta)\right)$, there are precisely $n$ different complex numbers. Let $w_0,~w_1,\ldots,~w_{n-1}$ be $n^{\text{th}}$ roots of $z$.

In particular, let $w = r e^{i\,\alpha}=r\left(\cos(\alpha)+i\sin(\alpha)\right)$ be one of these $n^{\text{th}}$ roots of $z$. In other words,
\begin{align*}
\textcolor{blue}{w^n} &= \textcolor{green}{z}\\
\textcolor{blue}{\left(r e^{i\,\alpha}\right)^n} &= \textcolor{green}{|z|\left(\cos(\theta) +i\sin(\theta)\right)}\\
\textcolor{blue}{r^n \left(\cos(n\alpha)+i\sin(n\alpha)\right)} &= \textcolor{green}{|z|\left(\cos(\theta) +i\sin(\theta)\right)}.
\end{align*}
It follows from the last equality that $\textcolor{blue}{r^n}=\textcolor{green}{|z|}$ and
$\begin{cases}
\textcolor{blue}{\cos(n\alpha)}=\textcolor{green}{\cos(\theta)},\\
\textcolor{blue}{\sin(n\alpha)}=\textcolor{green}{\sin(\theta)}.
\end{cases}$
This means $\alpha=\theta+2k\pi$, for $k$ an integer. Therefore,
\begin{align*}
\begin{cases}\textcolor{blue}{r}=\textcolor{green}{|z|^{1/n}},
\\ \vspace{-0.5cm}\\
\textcolor{blue}{\alpha} = \textcolor{green}{\dfrac{\theta+2k\pi}{n}},
\end{cases}
\end{align*}
and the $n^{\text{th}}$ root of $z$ are of the form
\begin{align*}
&|z|^{1/n}\left(\cos\left(\frac{\theta+2k\pi}{n}\right)+i\sin\left(\frac{\theta+2k\pi}{n}\right)\right),&
k=0,1,2,\ldots,n-1.
\end{align*}

<div class="alert alert-block alert-success">
<font size="+1"><b>
Roots of A Complex Number:
</b></font>
    
Assume that $q$ is a nonzero complex number and $n$ is a positive integer. Then, all $n$ distinct $z$ roots such that $z^n = q$ can be find as follows,
\begin{align*}
w_k=&r^{1/n}e^{i\left(\theta+2k\pi\right)/n}\\
&=r^{1/n}\left(\cos\left(\frac{\theta+2k\pi}{n}\right)+i\sin\left(\frac{\theta+2k\pi}{n}\right)\right),&
k=0,1,2,\ldots,n-1,
\end{align*}
where $r=|q|$ and $w_k$ with $k=0,1,2,\ldots,n-1$ are $n$ distinct $n^{\text{th}}$ roots.
  
</div>

<div class="alert alert-block alert-warning">
<font size="+1"><b>
Remark:
</b></font>
    
Observe that each of the $n^{\text{th}}$ roots of has modulus $|w_k|=r^{1/n}$. Therefore, all the $n^{\text{th}}$ roots of lie on the circle of radius $r^{1/n}$ in the complex plane.   
</div>

<font color='Blue'><b>Example</b></font>:
Find the six sixth roots of $-8$ and graph these roots in the complex plane.

<font color='Green'><b>Solution</b></font>: 
First of all, we need to write down $-8$ in $e^{i\theta}$ form. It can be seen that
\begin{align*}
r=|z|=\sqrt{(-8)^2}=|-8|=8 \quad \text{and}\quad
\begin{cases}
\cos(\theta)=\dfrac{-8}{8}=-1,\\
\sin(\theta)=\dfrac{0}{8}=0.
\end{cases}
\end{align*}

As the the principal argument $\theta \in (- \pi , \pi]$, $\theta=\pi.$.

Therefore, $-8=8e^{i\pi} $.
Since the argument is not unique, we can replace,
$\pi$ with $\pi+2\pi k$ for $k=0,1,2,\ldots,5$. We can find the roots using
\begin{align*}
&z^6=8e^{i\left(\pi+2\pi k\right)}, & k=0,1,2,\ldots,5,\\
\Rightarrow \quad &\sqrt[6]{z^6}=\sqrt[6]{8e^{i\left(\pi+2\pi k\right)}},& k=0,1,2,\ldots,5,\\
 \Rightarrow \quad &z=\sqrt[6]{8}e^{i\left(\pi+2\pi k\right)/6},& k=0,1,2,\ldots,5. \\
 \Rightarrow \quad &z=\sqrt{2}e^{i\left(\pi+2\pi k\right)/6},& k=0,1,2,\ldots,5.
\end{align*}

| $k$ 	| $0$ 	| $1$ 	| $2$ 	| $3$ 	| $4$ 	| $5$ 	|
|:-:	|:-:	|:-:	|:-:	|:-:	|:-:	|:-:	|
| $\theta$ 	| $\dfrac{\pi+2\pi(0)}{6}=\dfrac{\pi}{6}$ 	| $\dfrac{\pi+2\pi(1)}{6}=\dfrac{\pi}{2}$ 	| $\dfrac{\pi+2\pi(2)}{6}=\dfrac{5\pi}{6}$ 	| $\dfrac{\pi+2\pi(3)}{6}=\dfrac{7\pi}{6}$ 	| $\dfrac{\pi+2\pi(4)}{6}=\dfrac{3\pi}{2}$ 	| $\dfrac{\pi+2\pi(5)}{6}=\dfrac{11\pi}{6}$ 	|

Therefore,
\begin{align*}
&k=0
& w_0=&\sqrt{2}\left(\cos\left(\frac{\pi}{6}\right)+i\sin\left(\frac{\pi}{6}\right)\right)=
\sqrt{2}\left(\frac{\sqrt{3}}{2}+\frac{1}{2}i\right),
\\
&k=1
& w_1=&\sqrt{2}\left(\cos\left(\frac{\pi}{2}\right)+i\sin\left(\frac{\pi}{2}\right)\right)=
\sqrt{2}i,
\\
&k=2
& w_2=&\sqrt{2}\left(\cos\left(\frac{5\pi}{6}\right)+i\sin\left(\frac{5\pi}{6}\right)\right)=
\sqrt{2}\left(-\frac{\sqrt{3}}{2}+\frac{1}{2}i\right),
\\
&k=3
& w_3=&\sqrt{2}\left(\cos\left(\frac{7\pi}{6}\right)+i\sin\left(\frac{7\pi}{6}\right)\right)=
\sqrt{2}\left(-\frac{\sqrt{3}}{2}-\frac{1}{2}i\right),
\\
&k=4
& w_4=&\sqrt{2}\left(\cos\left(\frac{3\pi}{2}\right)+i\sin\left(\frac{3\pi}{2}\right)\right)=
-\sqrt{2}i,
\\
&k=5
& w_5=&\sqrt{2}\left(\cos\left(\frac{11\pi}{6}\right)+i\sin\left(\frac{11\pi}{6}\right)\right)=
\sqrt{2}\left(\frac{\sqrt{3}}{2}-\frac{1}{2}i\right).
\end{align*}

<center>
<iframe src="https://www.geogebra.org/classic/e9wq9bf9?embed" width="600" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>
</center>

***
**Refrences**
1. Kuttler, Kenneth. "A First Course in Linear Algebra (Lyryx)." (2018).
1. Nicholson, W. Keith. "Linear Algebra with Applications (Lyryx)." (2018).
1. Stewart, James, Daniel K. Clegg, and Saleem Watson. Calculus: early transcendentals. Cengage Learning, 2020.
***
