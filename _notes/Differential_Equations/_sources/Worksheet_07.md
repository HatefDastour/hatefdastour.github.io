# Worksheet 07

<div class="alert alert-block alert-success">
<font size="+0"><b>
The Abel's formula
</b></font>
    
<p>Suppose <span class="math inline">\(p(x)\)</span> and <span class="math inline">\(q(x)\)</span> are continuous on <span class="math inline">\((a,b),\)</span> let <span class="math inline">\(y_1(x)\)</span> and <span class="math inline">\(y_2(x)\)</span> be solutions of <span class="math display">\[\label{eq:5.1.27}
y&#39;&#39;+p(x)y&#39;+q(x)y=0\]</span> on <span class="math inline">\((a,b)\)</span>, and define <span class="math display">\[\label{eq:5.1.28}
W=y_1y_2&#39;-y_1&#39;y_2.\]</span> Let <span class="math inline">\(x_0\)</span> be any point in <span class="math inline">\((a,b).\)</span> Then <span class="math display">\[\label{eq:5.1.29}
W(x)=W(x_0) e^{-\int^x_{x_0}p(t)\,
dt}, \quad a&lt;x&lt;b.\]</span> Therefore either <span class="math inline">\(W\)</span> has no zeros in <span class="math inline">\((a,b)\)</span> or <span class="math inline">\(W\equiv0\)</span> on <span class="math inline">\((a,b).\)</span></p>
</div>



1. Find the Wronskian $W$ of a set of four solutions of 
\begin{align*}y^{(4)}+(\tan x)y'''+x^2y''+2xy=0,\end{align*}
given that $W(\pi/4)=K$.
    
<font color='Green'><b>Solution</b></font>:

From Abel's formula, $W(x)=W(\pi/2)\exp\left(-\int_{\pi/4}^x\tan t\,dt\right)$, where
\begin{align*}\int_{\pi/4}^x \tan t\,dt=-\ln(\sqrt2\cos x).\end{align*}
Therefore,
\begin{align*}W(x)=\sqrt2K\cos x.\end{align*}


***

2. Compute the Wronskian of the given set of functions.
* a). $\{e^x,\, e^x\sin x,\,e^x\cos x\}$
* b). ${\{1,\,x,\,{x^2\over2!},\,{x^3\over3!}\,,\cdots,\,{x^n\over n!}}\}$
* c). $\{e^x/x,\,e^{-x}/x,\,1\}$

<font color='Green'><b>Solution</b></font>:
* a). 
\begin{align*}
W(x)&=\left|\begin{array}{ccc}e^x&e^x\sin x&e^x\cos x\\e^x&e^x(\cos
x+\sin x)&
e^x(\cos x-\sin x)\\e^x&2e^x\cos x&-2e^x\sin x\end{array}\right|
=e^{3x}\left|\begin{array}{ccc}1&\sin x&\cos x\\1&\cos x+\sin x&
\cos x-\sin x\\1&2\cos x&-2\sin x\end{array}\right|
\\
&=e^{3x}\left|\begin{array}{ccc}1&\sin x&\phantom{-}\cos x\\0&\cos x&
-\sin x\\1&2\cos x-\sin x&-2\sin x-\cos x\end{array}\right|
=e^{3x}\left|\begin{array}{crr}1&\sin x&\cos x\\0&\cos x&
-\sin x\\0&-\sin x&-\cos x\end{array}\right|=-e^{3x}
\end{align*}

* b). 
$W(x)=
\left|\begin{array}{cccccc}
1&x&x^2/2&x^3/3&\cdots&x^n/n!\\
0&1&x&x^2/2&\cdots&x^{n-1}/(n-1)!\\
0&0&1&x&\cdots&x^{n-2}/(n-2)!\\
0&0&0&1&\cdots&x^{n-3}/(n-3)!\\
\vdots&\vdots&\vdots&\vdots&\ddots&\vdots\\
0&0&0&0&\cdots&1
\end{array}\right|=1$

* c). 
\begin{align*}
W(x)&=\left|\begin{array}{ccc}e^x/x&e^{-x}/x&1\\
e^x/x-e^x/x^2&-e^{-x}/x-e^{-x}/x^2&0\\
e^x/x-2e^x/x^2+2e^x/x^3&e^{-x}/x+2e^{-x}/x^2+2e^{-x}/x^3&0
\end{array}\right|
\\ &
= \left|\begin{array}{ccc}1/x&1/x&1\\
1/x-1/x^2&-1/x-1/x^2&0\\
1/x-2/x^2+2/x^3&1/x+2/x^2+2/x^3&0
\end{array}\right|
\\ &
=\left|\begin{array}{cc}
1/x-1/x^2&-1/x-1/x^2\\
1/x-2/x^2+2/x^3&1/x+2/x^2+2/x^3
\end{array}\right|
\\ &
=\left|\begin{array}{cr}
1/x-1/x^2&-2/x\\
1/x-2/x^2+2/x^3&4/x^2
\end{array}\right|=2/x^2.
\end{align*}
***

<div class="alert alert-block alert-success">
<font size="+0"><b>
General solution for the second-order homogeneous linear ODE
</b></font>
    
<p>Consider the second-order homogeneous linear ODE with <u>constant</u> coefficients, <span class="math display">\[\label{eq2.1.01}
a_{2} y&#39;&#39;(x)+a_{1} y&#39;(x)+a_{0} y(x)=0,\]</span> where <span class="math inline">\(a_0,~a_1\)</span> and <span class="math inline">\(a_2\)</span> are arbitrary constants.</p>
<p>The <em>characteristic equation</em> corresponding to the ODE can be found as follows, <span class="math display">\[\label{HOL-eq.02}
a_{2} r^2+a_{1} r+a_{0}=0.\]</span></p>
<p>Let <span class="math inline">\(r_1\)</span> and <span class="math inline">\(r_2\)</span> be the two roots of this characteristic equation. The following cases can be considered to find a general solution for the corresponding ODE.</p>
<ol>
<li><p>The characteristic equation has <u>distinct</u> real roots: <span class="math inline">\(r_1\)</span> and <span class="math inline">\(r_2\)</span><br />
</p></li>
<li><p>The characteristic equation has a pair of complex roots: <span class="math inline">\(\alpha \pm \beta i\)</span><br />
</p></li>
<li><p>Let <span class="math inline">\(r_1\)</span> be a root of the characteristic equation with the multiplicity of <span class="math inline">\(2\)</span> (i.e. <span class="math inline">\(r_1=r_2\)</span>).<br />
</p></li>
</ol>
</div>



3. Find the general solution.
* a). $y''-4y'+5y=0$,
* b). $y''-4y'+4y=0$,
* c). $y''+6y'+10y=0$,
* d). $6y''-y'-y=0$, with  $y(0)=10$, and $y'(0)=0$.
    
<font color='Green'><b>Solution</b></font>:

* a).
$p(r)=r^2-4r+5=(r-2)^2+1$.

Since $r_1,r_2=2\pm i$, then
\begin{align*}y=e^{2x}(c_1 \cos x+c_2 \sin x).\end{align*}

* b).
$p(r)=r^2-4r+4=(r-2)^2$.

Since $r_1,r_2=2$, then
\begin{align*}y=e^{2x}(c_1+c_2x).\end{align*}

* c).
$p(r)=r^2+6r+10=(r+3)^2+1$.

Since $r_1,r_2=-3\pm i$, then
\begin{align*}y=e^{-3x}(c_1 \cos x+c_2 \sin x).\end{align*}

* d). $p(r)=6r^2-r-1=(2r-1)(3r+1)=6(r-1/2) (r+1/3)$. Thus,
\begin{align*}y=c_1e^{-x/3}+c_2e^{x/2}\end{align*}
Moreover,
$y'=-\dfrac{c_1}{3}e^{-x/3}+\dfrac{c_2}{2}e^{x/2}$. Now,
\begin{align*}\begin{cases}
  y(0)=10\Rightarrow c_1+c_2=10\\
  y'(0)=0\Rightarrow -{c_1\over3}+{c_2\over2}=0.
\end{cases}
\end{align*}
Hence, $c_1=6, c_2=4$, and $y=4e^{x/2}+6e^{-x/3}$.


***

4. Find a fundamental set of solutions of the given equation, and verify that it's a fundamental set by evaluating  its Wronskian at $x=0$.
* a). $(D-1)^2(D-2)y=0$,
* b). $(D^2+4)(D-3)y=0$,
* c). $(D^2+2D+2)(D-1)y=0$,
* d). $D^3(D-1)y=0$,
* e). $(D^2-1)(D^2+1)y=0$,
* f). $(D^2-2D+2)(D^2+1)y=0$.

<font color='Green'><b>Solution</b></font>:

* a). First off,
$W(x)=\left|\begin{array}{ccc}
e^x&xe^x&e^{2x}\\
e^x&e^x(x+1)&2e^{2x}\\
e^x&e^x(x+2)&4e^{2x}
\end{array}\right|$.

Moreover,

\begin{align*}W(0)=\left|\begin{array}{cccc}
1&0&1\\1&1&2\\1&2&4
\end{array}\right|=
\left|\begin{array}{cccc}
1&0&0\\1&1&1\\1&2&3
\end{array}\right|
=\left|\begin{array}{cccc}
1&1\\2&3\end{array}\right|=1.
\end{align*}

* b).
$
W(x)=\left|\begin{array}{ccc}
\cos 2x&\sin 2x&e^{3x}\\
-2\sin 2x&2\cos 2x&3e^{3x}\\
-4\cos 2x&-4\sin 2x&9e^{3x}
\end{array}\right|.$
Also,
\begin{align*}
W(0)=\left|\begin{array}{rccc}
1&0&1\\0&2&3\\-4&0&9
\end{array}\right|=
\left|\begin{array}{rccc}
1&0&0\\0&2&3\\-4&0&13
\end{array}\right|=
\left|\begin{array}{rccc}
2&3\\0&13\end{array}\right|=26.
\end{align*}

* c).
We have,
$
W(x)=\left|\begin{array}{ccc}
e^{-x}\cos x&e^{-x}\sin x&e^x\\
-e^{-x}(\cos x+\sin x)&e^{-x}(\cos x-\sin x)&e^x\\
2e^{-x}\sin x&-2e^{-x}\cos x&
e^x\end{array}\right|.
$
In addition,
\begin{align*}
W(0)=\left|\begin{array}{rrc}
1&0&1\\-1&1&1\\0&-2&1
\end{array}\right|=
\left|\begin{array}{rrc}
1&0&1\\0&1&2\\0&-2&1
\end{array}\right|=
\left|\begin{array}{rcc}
1&2\\-2&1\end{array}\right|=5.
\end{align*}

* d).
$
W(x)=\left|\begin{array}{cccc}
1&x&x^2&e^x\\
0&1&2x&e^x\\0&0&2&e^x\\0&0&0&e^x\end{array}\right|.
$
Also,
$
W(0)=\left|\begin{array}{cccc}
1&0&0&1\\0&1&0&1\\0&0&2&1\\0&0&0&1
\end{array}\right|=1.
$

* e).
First off,
$W(x)=\left|\begin{array}{rrrr}e^x&e^{-x}&\cos x&\sin x\\
e^x&-e^{-x}&-\sin x&\cos x\\e^x&e^{-x}&-\cos x&-\sin
x\\e^x&-e^{-x}&\sin x&-\cos x\end{array}\right|.
$
\begin{eqnarray*}
W(0)&=&\left|\begin{array}{rrrr}
1&1&1&0\\1&-1&0&1\\1&1&-1&0\\1&-1&0&-1
\end{array}\right|
=\left|\begin{array}{rrrr}
1&1&1&0\\1&-1&0&1\\1&1&-1&0\\0&0&0&-2
\end{array}\right|
=-2\left|\begin{array}{rrrr}
1&1&1\\1&-1&0\\1&1&-1\\
\end{array}\right|\\
&=&-2\left|\begin{array}{rrrr}
1&1&1\\1&-1&0\\0&0&-2\\
\end{array}\right|
=4\left|\begin{array}{rrrr}
1&1\\1&-1\\\end{array}\right|=-8.
\end{eqnarray*}

* f).
We have,
$
W(x)=\left|\begin{array}{rrcc}\cos x&\sin x&e^x\cos x&e^x\sin x\\
-\sin x&\cos x&e^x(\cos x-\sin x)&e^x(\cos x+\sin x)\\
-\cos x&-\sin x&-2e^x\sin x&2e^x\cos x\\
\sin x&-\cos x&-e^x(2\cos x+2\sin x)&e^x(2\cos x-2\sin x)
\end{array}\right|.
$

Moreover,
\begin{eqnarray*}
W(0)&=&\left|\begin{array}{rrrr}
1&0&1&0\\0&1&1&1\\-1&0&0&2\\0&-1&-2&2
\end{array}\right|=
\left|\begin{array}{rrrr}
1&0&1&0\\0&1&1&1\\0&0&1&2\\0&-1&-2&2
\end{array}\right|=
\left|\begin{array}{rrrr}
1&1&1\\0&1&2\\-1&-2&2
\end{array}\right|\\
&=&\left|\begin{array}{rrrr}
1&1&1\\0&1&2\\0&-1&3
\end{array}\right|=
\left|\begin{array}{rrrr}
1&1&1\\0&1&2\\0&0&5
\end{array}\right|=5.
\end{eqnarray*}

***
## Refrences
1. Trench, William F. "Elementary differential equations with boundary value problems." (2018).
***
