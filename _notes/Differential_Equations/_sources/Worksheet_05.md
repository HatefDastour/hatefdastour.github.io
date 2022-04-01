# Worksheet 05

<div class="alert alert-block alert-success">
<font size="+0"><b>
Theorem 2.6.1 from the textbook
</b></font>
    
<p>Consider the following ODE <span class="math display">\[\label{eq:2.6.11}
M(x,y)\,dx+N(x,y)\,dy=0,\]</span> where <span class="math inline">\(M,\)</span> <span class="math inline">\(N,\)</span> <span class="math inline">\(M_y,\)</span> and <span class="math inline">\(N_x\)</span> be continuous on an open rectangle <span class="math inline">\(\mathbb{R}.\)</span> Then<span class="math inline">\(:\)</span></p>
<ol>
<li><p>If <span class="math inline">\((M_y-N_x)/N\)</span> is independent of <span class="math inline">\(y\)</span> on <span class="math inline">\(R\)</span> and we define <span class="math inline">\(p(x)=\frac{M_y-N_x}{N},\)</span> then <span class="math display">\[\label{eq:2.6.10}
\mu(x)=\pm e^{\int p(x)\,dx}\]</span> is an integrating factor for the ODE on <span class="math inline">\(R.\)</span></p></li>
<li><p>If <span class="math inline">\((N_x-M_y)/M\)</span> is independent of <span class="math inline">\(x\)</span> on <span class="math inline">\(R\)</span> and we define <span class="math inline">\(q(y)=\frac{N_x-M_y}{M},\)</span> then <span class="math display">\[\label{eq:2.6.12}
\mu(y)=\pm e^{\int q(y)\,dy}\]</span> is an integrating factor for the ODE on <span class="math inline">\(\mathbb{R}.\)</span></p></li>
</ol>
</div>

1. Find an integrating factor, and solve the given equation.
\begin{align*}(5xy+2y+5)\,dx+2x\,dy=0.\end{align*}
    
<font color='Green'><b>Solution</b></font>:

Let $M(x,y) = 5xy+2y+5$ and $N(x,y) = 2x$. We have,
\begin{align*}
\frac{\partial M}{\partial y} - \frac{\partial N}{\partial x} =  5x.
\end{align*}

It can be seen that
\begin{align*}p(x) = \frac{1}{N(x,y)}\left( \frac{\partial M}{\partial y} - \frac{\partial N}{\partial x}\right) = \frac{5}{2}.\end{align*}

Thus, $\mu(x) = \exp\left(\int \frac{5}{2} dx\right) = \exp\left(\frac{5}{2} x\right) $.

Now, $\exp\left(\frac{5}{2} x\right)(5xy+2y+5)\,dx+\exp\left(\frac{5}{2} x\right)2x\,dy=0$ is exact!

To solve this exact equation. We need to identify $F(x,y) = c$ such that
* $\frac{\partial F}{\partial x} = \exp\left(\frac{5}{2} x\right)(5xy+2y+5)$,
* $\frac{\partial F}{\partial y} = \exp\left(\frac{5}{2} x\right)2x$.

It follows from $\frac{\partial F}{\partial y} = 2x\exp\left(\frac{5}{2} x\right)$ that

\begin{align*}
& F(x,y) = \int \left( 2x\exp\left(\frac{5}{2} x\right) \right) dy,\\
\Rightarrow \quad & F(x,y) = 2xy \exp\left(\frac{5}{2} x\right) +\psi(x).
\end{align*}

Now, to find $\psi(x)$, we can use $\frac{\partial F}{\partial x} = \exp\left(\frac{5}{2} x\right)(5xy+2y+5)$. This means,

\begin{align*}
2y \exp\left(\frac{5}{2} x\right) + 5xy \exp\left(\frac{5}{2} x\right) +\psi'(x) = \exp\left(\frac{5}{2} x\right)(5xy+2y+5).
\end{align*}

It follows that
\begin{align*}\psi'(x)= 5  \exp\left(\frac{5}{2} x\right).\end{align*}
and
\begin{align*}
\psi(x)= 2  \exp\left(\frac{5}{2} x\right).
\end{align*}
Therefore, 
\begin{align*}2xy \exp\left(\frac{5}{2} x\right) + 2  \exp\left(\frac{5}{2} x\right)=c, \quad c \in \mathbb{R}.\end{align*}


***

2. Find an integrating factor of the form $\mu(x,y)=P(x)Q(y)$ and solve the following equation.
\begin{align*}2y\,dx+ 3(x^2+x^2y^3)\,dy=0.\end{align*}
    
<font color='Green'><b>Solution</b></font>:
Let $M(x,y) = 2y$ and $N(x,y) = 3(x^2+x^2y^3)$. Then,
\begin{align*}
\frac{\partial M}{\partial y} - \frac{\partial N}{\partial x} =  2- (6x+6xy^3).
\end{align*}

Now, let $\mu(x,y)=P(x)Q(y)$ be an integrating factor, and $p(x)$ and $q(y)$ be two functions such that 
* $\frac{\partial M}{\partial y} - \frac{\partial N}{\partial x} = p(x)N(x,y) - q(y)M(x,y)$,
* $P(x) = \exp\left( \int p(x) dx \right)$,
* $Q(y) = \exp\left( \int q(y) dy \right)$.

It follows that
\begin{align*}2-(6x +6xy^3) = 3x p(x) (x+xy^3) -2yq(y).\end{align*}

Let $xp(x) = a$ and $yq(y) = b$. Then,
\begin{align*}2-6x -6xy^3 = 3a (x+xy^3) -2b.\end{align*}

It follows that $a = -2$ and $b = -1$. Therefore, $p(x) = -2/x$ and $q(x) = -1/y$ and

* $P(x) = \exp\left( \int p(x) dx \right) = \frac{1}{x^2}$,
* $Q(y) = \exp\left( \int q(y) dy \right) = \frac{1}{y}$.

Now,
\begin{align*}\mu(x,y)=P(x)Q(y) = \frac{1}{x^2y}.\end{align*}
To solve this exact equation. We need to identify $F(x,y) = c$ such that
* $\frac{\partial F}{\partial x} = \frac{2}{x^2}$,
* $\frac{\partial F}{\partial y} = 3\left( \frac{1}{y} + y^2 \right)$.

It follows from $\frac{\partial F}{\partial x} = \frac{2}{x^2}$ that

\begin{align*}
& F(x,y) = -\frac{2}{x} +\psi(y).
\end{align*}

Now, to find $\psi(y)$, we can use $\frac{\partial F}{\partial y} = 3\left( \frac{1}{y} + y^2 \right)$. This means,

\begin{align*}
\psi'(y) = 3\left( \frac{1}{y} + y^2 \right).
\end{align*}

It follows that
\begin{align*}
\psi(x)= y^3 + \ln|y|.
\end{align*}
Therefore, 
\begin{align*}-\frac{2}{x} + y^3 + \ln|y|=c, \quad c \in \mathbb{R}.\end{align*}

***
## Refrences
1. Trench, William F. "Elementary differential equations with boundary value problems." (2018).
***