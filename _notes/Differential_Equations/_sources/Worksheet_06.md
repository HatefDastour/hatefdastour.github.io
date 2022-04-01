# Worksheet 06

1. Compute the Wronskians of the given sets of functions.

* a). $\{e^x, e^x \sin x\}$,
* b). $\{ x^{1/2},  x^{-1/3}\}$.
    
<font color='Green'><b>Solution</b></font>:

* a). 
\begin{align*}
W(x)=\begin{vmatrix}
e^x & e^x \sin x \\
e^x & e^x\,\cos\left(x\right)+e^x\,\sin\left(x\right)
\end{vmatrix}=e^{2\,x}\,\cos\left(x\right).
\end{align*}
* b). 

\begin{align*}
W(x)=\begin{vmatrix}
\sqrt{x} & \frac{1}{x^{1/3}}\\ \frac{1}{2\,\sqrt{x}} & -\frac{1}{3\,x^{4/3}}
\end{vmatrix}=-\frac{5}{6\,x^{5/6}}.
\end{align*}


***

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



2. Find the Wronskian of a given set $\{y_1,y_2\}$ of solutions of
\begin{align*}
x^2y''+xy'+(x^2-\nu^2)y=0 ,
\end{align*}
given that $W(1)=1$.
    
<font color='Green'><b>Solution</b></font>:

Note that $p(x)=\dfrac{1}{x}$. Thus,
\begin{align*}
\int^x_{x_0}p(t)\,dt= {\int_1^x  p(t)\,dt}={\int_1^x\frac{1}{t}dt}=\ln x,\end{align*}
and Abel's
formula yields
\begin{align*}W(x)=W(1)e^{-\ln x}=\frac{1}{x}.\end{align*}


***

<div class="alert alert-block alert-success">
<font size="+0"><b>
Fundamental Set of Solutions
</b></font>
    
<p>Suppose <span class="math inline">\(p\)</span> and <span class="math inline">\(q\)</span> are continuous and <span class="math inline">\(y_1\)</span> is a solution of <span class="math display">\[y&#39;&#39;+p(x)y&#39;+q(x)y=0\qquad (A)\]</span> that has no zeros on <span class="math inline">\((a,b)\)</span>. Let <span class="math inline">\(P(x)=\int p(x)\,dx\)</span> be any antiderivative of <span class="math inline">\(p\)</span> on <span class="math inline">\((a,b)\)</span>.</p>
<ol>
<li><p>If <span class="math inline">\(K\)</span> is an arbitrary nonzero constant and <span class="math inline">\(y_2\)</span> satisfies <span class="math display">\[y_1y_2&#39;-y_1&#39;y_2=Ke^{-P(x)}
\qquad (B)\]</span> on <span class="math inline">\((a,b)\)</span>, then <span class="math inline">\(y_2\)</span> also satisfies (A) on <span class="math inline">\((a,b)\)</span>, and <span class="math inline">\(\{y_1,y_2\}\)</span> is a fundamental set of solutions on (A) on <span class="math inline">\((a,b)\)</span>.</p></li>
<li><p>If <span class="math inline">\(y_2=uy_1\)</span> where <span class="math inline">\(u&#39;=K\dfrac{e^{-P(x)}}{y_1^2(x)}\)</span>, then <span class="math inline">\(\{y_1,y_2\}\)</span> is a fundamental set of solutions of (A) on <span class="math inline">\((a,b)\)</span>.</p></li>
</ol>
</div>



3. For the given ODE, find a second solution $y_2$ that isn't a constant multiple of the solution $y_1$. Choose $K$ conveniently to simplify
$y_2$.

* a). $y''-2ay'+a^2y=0,\quad (a=\text{ constant, and })  \quad  y_1=e^{ax}$
* b).  $x^2y''-xy'+y=0,  \quad y_1=x$
    
<font color='Green'><b>Solution</b></font>:

* a). We can see that $p(x)=-2a$. Then, $P(x)= \int p(x)\,dx = -2ax$. Moreover, letting
$y_2=uy_1=ue^{ax}$, leads to
\begin{align*}u'=K\frac{e^{-P(x)}}{y_1^2(x)}=K\frac{e^{2ax}}{ e^{2ax}}=K.\end{align*}
Therefore, $u=\int K~dx=Kx$.

As $K$ is an arbitrary nonzero constant, choosing $K=1$ gives 
\begin{align*}
y_2=xe^{ax}.
\end{align*}

* b). Here, $p(x)=-{1\over x}$, then $P(x)=-\ln x$. Moreover, let
$y_2=uy_1=ux$. It follows that
\begin{align*}u'=K \frac{e^{-P(x)}}{ y_1^2(x)}=K\frac{x}{ x^2}={K}\frac{1}{ x}.\end{align*}
Thus, $u=K\ln x$. Letting $K=1$, then $y_2=x\ln x$.


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



4. Find the general solution.
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
\begin{align*}
y=c_1e^{-x/3}+c_2e^{x/2}
\end{align*}
Moreover,
$y'=-\dfrac{c_1}{3}e^{-x/3}+\dfrac{c_2}{2}e^{x/2}$. Now,
\begin{align*}\begin{cases}
  y(0)=10\Rightarrow c_1+c_2=10\\
  y'(0)=0\Rightarrow -{c_1\over3}+{c_2\over2}=0.
\end{cases}
\end{align*}
Hence, $c_1=6, c_2=4$, and $y=4e^{x/2}+6e^{-x/3}$.


***
## Refrences
1. Trench, William F. "Elementary differential equations with boundary value problems." (2018).
***
