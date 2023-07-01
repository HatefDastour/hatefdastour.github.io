# Worksheet 01

1. Find the order of the equation.
* *a)* $\dfrac{d^2y}{dx^2}+2\dfrac{dy}{dx}\,\dfrac{d^3y}{dx^3}+x=0$
* *b)* $y''-3y'+2y=x^7$
* *c)* $y'-y^7=0$
* *d)* $y''y-(y')^2=2$
    
<font color='Green'><b>Solution</b></font>:

* *a)* 3
* *b)* 2
* *c)* 1
* *d)* 2
***

2. Verify that the  function is a solution of the differential equation on some interval, for any choice of the arbitrary constants appearing in the function.
* *a)* $y=ce^{2x};     \quad y'=2y$
* *b)* $y=\dfrac{x^2}{3}+\dfrac{c}{x};   \quad xy'+y=x^2$

    
<font color='Green'><b>Solution</b></font>:

* *a)* If $y=ce^{2x}$, then $y'=2ce^{2x}=2y$.

* *b)* If $y= {x^2\over3}+{c\over x}$, then
\begin{align*}
& y'={2x\over3}-{c\over x^2},\\
\Rightarrow \quad & xy'+y={2x^2\over3}-{c\over x}+{x^2\over3}+{c\over x}=x^2.
\end{align*}
***

3. Find all solutions of the equation.
* *a)* $y'=-x$
* *b)* $y'=-x \sin (x)$
* *c)* $y''=2xe^x$
    
<font color='Green'><b>Solution</b></font>:

* *a)* 
\begin{align*}
& y'=-x,\\
\Rightarrow \quad & \frac{dy}{dx} = -x,\\
\Rightarrow \quad & dy = -x\,dx,\\
\Rightarrow \quad & \int dy = \int-x\,dx,\\
\Rightarrow \quad & y=-\frac{x^2}{2}+c,\quad c \in \mathbb{R}.
\end{align*}

* *b)* 
\begin{align*}
& y'=-x \sin (x),\\
\Rightarrow \quad & \frac{dy}{dx} = -x \sin (x),\\
\Rightarrow \quad & dy = -x \sin (x)dx,\\
\Rightarrow \quad & \int dy = \int-x \sin (x)dx,\\
\Rightarrow \quad & y=x\cos x- \sin( x) +c.,\quad c \in \mathbb{R}.
\end{align*}
* *c)* 
\begin{align*}
& y''=2xe^x,\\
\Rightarrow \quad & \int y''=\int 2xe^x,\\
\Rightarrow \quad & y'= 2x e^{x} - 2 e^{x} + c_1,\quad c_1 \in \mathbb{R},\\
\Rightarrow \quad & \int y'= \int \left(2x e^{x} - 2 e^{x} + c_1\right),\quad c_1 \in \mathbb{R},\\
\Rightarrow \quad & y = (2x - 4)e^{x} + c_1 + c_2 x,\quad c_1,c_2 \in \mathbb{R}.
\end{align*}

***

4. Solve the  initial value problem

* *a)* $y'=\tan(x), \quad y(\pi/4)=3$
* *b)* $y''=x^4, \quad y(2)=-1, \quad y'(2)=-1$
* *c)* $y'''=2+\sin 2x, \quad y(0)=1, \quad y'(0)=-6, \quad y''(0)=3$

<font color='Green'><b>Solution</b></font>:

* *a)* 

We have
\begin{align*}y'=\tan(x)={\sin(x)\over\cos(x)}=-{1\over\cos(x)}{d\over dx}(\cos(x)).\end{align*}
Integrating both sides yields 
\begin{align*}y=-\ln|\cos(x)|+c,\quad c \in \mathbb{R}.\end{align*}
Now, since $y(\pi/4)=3$, we have,
\begin{align*}
& 3=-\ln\left(\cos(\pi/4)\right)+c,\\
\Rightarrow \quad & 3=\ln\sqrt2+c,\\
\Rightarrow \quad & c=3-\ln\sqrt{2},\\
\Rightarrow \quad & y=-\ln(|\cos(x)|)+3-\ln\sqrt2=3-\ln(\sqrt2|\cos(x)|).
\end{align*}

* *b)* 
\begin{align*}
& y''=x^4,\\
\Rightarrow \quad & y'=\frac{x^5}{5}+c_1, \quad c_1 \in \mathbb{R}
\end{align*}
Now, since $y'(2)=-1$,
\begin{align*}
& \frac{32}{5} + c_1 = -1,\\
\Rightarrow \quad &  c_1=-{37\over15}.
\end{align*}
It follows that,
\begin{align*}
& y'={x^5\over5}-{37\over15},\\
\Rightarrow \quad & y'=\frac{x^5}{5}+c_1, \quad c_1 \in \mathbb{R},\\
\Rightarrow \quad & y= \frac{x^6}{30}- \frac{37}{15}(x-2)+c_2,\quad c_1,c_2 \in \mathbb{R}.
\end{align*}
Since $y(2)=-1$,
\begin{align*}
& \frac{64}{30}+c_2=-1,\\
\Rightarrow \quad & c_2=-\frac{47}{15},
\end{align*}
Therefore,
\begin{align*}y=-\frac{47}{15}-\frac{37}{5}(x-2)+\frac{x^6}{30}.\end{align*}

* *c)* 
\begin{align*}
& y'''=2+\sin(2x),\\
\Rightarrow \quad & y''=2x- \frac{\cos 2x}{2}+c_1,\quad c_1 \in \mathbb{R}.
\end{align*}

Now, it follows from $y''(0)=3$,
\begin{align*}
& -\frac{1}{2}+c_1=3,\\
\Rightarrow \quad & c_1={7\over2},\\
\Rightarrow \quad & y''=2x- \frac{\cos (2x)}{2}+ \frac{7}{2}.
\end{align*}

Next,
\begin{align*}
y'=x^2- \frac{\sin 2x}{4}+ \frac{7}{2}x+c_2,\quad c_2 \in \mathbb{R}.
\end{align*}

Moreover, since $y'(0)=-6$, we have $c_2=-6$. Thus,
\begin{align*}
& y'=x^2- \frac{\sin (2x)}{4}+ \frac{7}{2}x-6,\\
\Rightarrow \quad & y= \frac{x^3}{3}+ \frac{\cos (2x)}{8}+ \frac{7}{4}x^2-6x+c_3,\quad c_3 \in \mathbb{R}.
\end{align*}

It follows from $y(0)=1$,
\begin{align*}
& \frac{1}{8}+c_3=1,\\
\Rightarrow \quad & c_3= \frac{7}{8},\\
\Rightarrow \quad & y= \frac{x^3}{3}+ \frac{\cos (2x)}{8}+ \frac{7}{4}x^2-6x+ \frac{7}{8}.
\end{align*}

***
**Refrences**

1. Trench, William F. "Elementary differential equations with boundary value problems." (2018).
***