# Worksheet 09

`````{admonition} Power Series
:class: important

For any power series of the form:

\begin{align*}
\sum_{n=0}^\infty a_n(x-x_0)^n,
\end{align*}

exactly one of the following statements is true:

* (i) The power series converges only for $x=x_0$.
* (ii) The power series converges for all values of $x$.
* (iii) There exists a positive number $R$ such that the power series converges if $|x-x_0|<R$ and diverges if $|x-x_0|>R$.

In case (iii), we refer to $R$ as the \textcolor{blue}{radius of convergence} of the power series. For convenience, we include the other two cases in this definition by defining $R=0$ in case (i) and $R=\infty$ in case (ii). We define the \textcolor{blue}{open interval of convergence} of $\sum_{n=0}^\infty a_n(x-x_0)^n$ as follows:

\begin{align*}
(x_0-R,x_0+R) \quad \text{if} \quad 0<R<\infty, \quad \text{or} \quad (-\infty,\infty) \quad \text{if} \quad R=\infty.
\end{align*}

If $R$ is finite, no general statement can be made regarding the convergence at the endpoints $x=x_0\pm R$ of the open interval of convergence. The series may converge at one or both points, or diverge at both.
`````

1. For each power series, find the radius of convergence $R$. If $R>0$, find the open interval of convergence.

* a)  ${\sum_{n=0}^\infty {(-1)^n\over2^nn}(x-1)^n}$
* b)  ${\sum_{n=0}^\infty 2^nn(x-2)^n}$
* c)  ${\sum_{n=0}^\infty {n!\over9^n}x^n}$
* d)  ${\sum_{n=0}^\infty{n(n+1)\over16^n}(x-2)^n}$
* e)  ${\sum_{n=0}^\infty (-1)^n{7^n\over n!}x^n}$
* f)  ${\sum_{n=0}^\infty {3^n\over4^{n+1}(n+1)^2}(x+7)^n}$
* g) ${\sum_{n=0}^\infty {n!\over9^n}x^n}$
* h)  ${\sum_{n=0}^\infty (-1)^n{7^n\over n!}x^n}$

<font color='Green'><b>Solution</b></font>:

* a) We have
\begin{align*}L = \lim_{n\to\infty}\left|a_{n+1}\over a_n\right| =\frac{\frac{(-1)^{n+1}}{2^{n+1}(n+1)}}{\frac{(-1)^{n}}{2^{n}n}} = 2,\end{align*}
Thus,
$R = 2$, $I = (1-2,1+2) = (-1,3)$,
* b)  Similarly,
\begin{align*}L = \lim_{n\to\infty}\left|a_{n+1}\over a_n\right| =\frac{2^{n+1}}{2^n} = 2,\end{align*}
Thus,
$R = 1/2$, $I = (2-1/2,2+1/2) = (3/2,5/2)$,
* c)  We have,
\begin{align*}
L = \lim_{n\to\infty}\left|a_{n+1}\over a_n\right| =\frac{\frac{(n+1)!}{9^{n+1}}}{\frac{n!}{9^{n}}} = \frac{n+1}{9} =\infty,
\end{align*}
Thus,$R = 0$,
* d)  $R = 16$, $I = (-14;18)$,
* e)  We have,
\begin{align*}L = \lim_{n\to\infty}\left|a_{n+1}\over a_n\right| =\frac{\frac{7^{n+1}}{(n+1)!}}{\frac{7^n}{n!}} = \frac{7}{n+1} =0,
\end{align*}
Therefore, $R = \infty$, $I = (-\infty,\infty)$,
* f)  $R = 4/3$, $I = (-25/3,-17/3)$.
* g)  $R = 0$,
* h)  $R = \infty$, $I = (-\infty,\infty)$,
***

`````{admonition} Theorem

\textbf{Theorem 7.2.2}: Consider the coefficients $\{a_n\}$ in any solution of the form $y=\sum_{n=0}^\infty a_n(x-x_0)^n$ for the differential equation:

\begin{equation}
\left(1+\alpha(x-x_0)^2\right)y''+\beta(x-x_0) y'+\gamma y=0 \quad \text{(1)}
\end{equation}

The coefficients satisfy the recurrence relation:

\begin{equation}
a_{n+2}=-\frac{p(n)}{(n+2)(n+1)}a_n, \quad n\geq 0 \quad \text{(2)}
\end{equation}

where

\begin{equation}
p(n)=\alpha n(n-1) +\beta n+\gamma \quad \text{(3)}
\end{equation}

Furthermore, the coefficients of the even and odd powers of $(x-x_0)$ can be computed separately as:

\begin{eqnarray}
a_{2m+2}&=&-\frac{p(2m)}{(2m+2)(2m+1)}a_{2m}, \quad m\geq 0 \quad \text{(4)}\\
a_{2m+3}&=&-\frac{p(2m+1)}{(2m+3)(2m+2)}a_{2m+1}, \quad m\geq 0 \quad \text{(5)}
\end{eqnarray}

Here, $a_0$ and $a_1$ are arbitrary.
`````



2. For the following ODE, find the power series in $x$ for the general solution.
\begin{align*}(1-x^2)y''-8xy'-12y=0.\end{align*}

<font color='Green'><b>Solution</b></font>:

Note that here  $\alpha=-1$, $\beta=-8$, and $\gamma=-12$. Therefore,
\begin{align*}p(n)=-n(n-1)-8n-12=-(n+3)(n+4)\end{align*}
Hence,
\begin{align*}a_{n+2}=-{(n+3)(n+4)\over(n+2)(n+1)}a_n\end{align*}
Writing this equation separately for $n=2m$  and $n=2m+1$ yields
\begin{align*}
a_{2m+2}&=-{(m+2)(2m+3)\over(m+1)(2m+1)}a_{2m}\\
a_{2m}&= -{((m-1)+2)(2(m-1)+3)\over((m-1)+1)(2(m-1)+1)} a_{2(m-1)}= \ldots = (m+1)(2m+1)a_0
\end{align*}
\begin{align*}
a_{2m+3} & = {(m+2)(2m+5)\over(m+1)(2m+3)}a_{2m+1}\\
a_{2m+1} & = {((m-1)+2)(2(m-1)+5)\over((m-1)+1)(2(m-1)+3)}a_{2(m-1)+1}= \ldots  = {(m+1)(2m+3)\over3}a_1
\end{align*}
Therefore, if  $m\ge0$;
\begin{align*}y={a_0\sum_{m=0}^\infty(m+1)(2m+1)x^{2m}+{a_1\over3}\sum_{m=0}^\infty
(m+1)(2m+3)x^{2m+1}}.\end{align*}
***

3. Find $a_0$, ..., $a_N$ for $N$ at least $7$ in the power series solution

\begin{align*}(1+2x^2)y''-9xy'-6y=0,\qquad y(0)=1,\quad y'(0)=-1\end{align*}

<font color='Green'><b>Solution</b></font>:

Since $\alpha=2$, $\beta=-9$, and $\gamma=-6$,
\begin{align*}p(n)=2n(n-1)-9n-6=(n-6)(2n+1).\end{align*}
Therefore
\begin{align*}
a_{n+2}=-{(n-6)(2n+1)\over(n+2)(n+1)}a_n,\quad n\ge0.
\end{align*}

Writing this equation separately for $n=2m$  and $n=2m+1$ yields

\begin{eqnarray}
a_{2m+2}&=&
-{(m-3)(4m+1)\over(m+1)(2m+1)}a_{2m}
,\quad m\ge
0\label{eq:7.2.30}\\
a_{2m+3}&=&
-{(2m-5)(4m+3)\over(2m+3)(2m+2)}a_{2m+1}
,\quad m\ge0.
\end{eqnarray}
Starting with  $a_0=y(0)=1$, we can compute $a_2, a_4$, and $a_6$:
\begin{eqnarray*}
a_2=3,~a_4=5,~a_6=3,
\end{eqnarray*}
Moreover, starting with $a_1=y'(0)=-1$, we can compute $a_3,a_5$ and $a_7$:

\begin{eqnarray*}
a_3,=-5/2,~a_5=-21/8,~a_7=-11/16
\end{eqnarray*}
Therefore, the solution is
\begin{align*}
y=1-x+3x^2-\frac{5}{2}x^3+5x^4-\frac{21}{8}x^5+3x^6-\frac{11}{16}x^7+\cdots\; .
\end{align*}
***

4. Find  the coefficients
$a_0$,\dots, $a_N$ for $N$ at least $7$ in the series solution
$y=\sum_{n=0}^\infty a_nx^n$ of the initial value problem.

* a)
$(1+x+2x^2)y''+(2+8x)y'+4y=0,\quad y(0)=-1,\quad y'(0)=2$
* b)
$(1-x+x^2)y''-(1-4x)y'+2y=0,\quad y(1)=2,\quad y'(1)=-1$

<font color='Green'><b>Solution</b></font>:

* a)
If $y=\sum_{n=0}^\infty a_nx^n$, then
\begin{align*}
(1+x+2x^2)y''&=
 \sum_{n=2}^\infty n(n-1)a_nx^{n-2}
+\sum_{n=2}^\infty n(n-1)a_nx^{n-1}
+2\sum_{n=2}^\infty n(n-1)a_nx^n,
\\
(2+8x)y' &=2\sum_{n=1}^\infty na_nx^{n-1}
+8\sum_{n=1}^\infty na_nx^n
\\
4y&=
4\sum_{n=0}^\infty a_nx^n
\end{align*}
Thus,
\begin{align*}
(1+x+2x^2)y''+(2+8x)y'+4y=\sum_{n=0}^\infty(n+2)(n+1)(a_{n+2}+a_{n+1}+2a_n)x^n=0.
\end{align*}
Now, if $a_{n+2}=-a_{n+1}-2a_n$, $a_n\ge0$. Starting with $a_0=-1$ and $a_1=2$ yields
\begin{align*}y={-1+2x-4x^3+4x^4+4x^5-12x^6+4x^7+\cdots}.\end{align*}

* b)
The equation is equivalent to $(1+t+t^2)y''+(3+4t)y'+2y=0$ with $t=x-1$. If $y=\sum_{n=0}^\infty a_nt^n$, then
\begin{align*}
(1+t+t^2)y''+(3+4t)y'+2y&=
 \sum_{n=2}^\infty n(n-1)a_nt^{n-2}
+\sum_{n=2}^\infty n(n-1)a_nt^{n-1}
+\sum_{n=2}^\infty n(n-1)a_nt^n
\\ &
+3\sum_{n=1}^\infty na_nt^{n-1}
+4\sum_{n=1}^\infty na_nt^n
\\ &
+2\sum_{n=0}^\infty a_nt^n
\\ &
=\sum_{n=0}^\infty(n+1)[(n+2)a_{n+2}+(n+3)a_{n+1}+(n+2)a_n]t^n=0
\end{align*}
if
$a_{n+2}=-{n+3\over n+2}a_{n+1}-a_n$,
$a_n\ge0$. Starting with $a_0=2$ and $a_1=-1$ yields
\begin{align*}
y & =2-(x-1)-{1\over2}(x-1)^2+{5\over3}(x-1)^3-{19\over12}(x-1)^4
\\&
+{7\over30}(x-1)^5+{59\over45}(x-1)^6-{1091\over630}(x-1)^7+\cdots
\end{align*}
***

`````{admonition} Theorem

Let's consider the given equations and rewrite the solution statement in a clearer manner:

Suppose the indicial equation is given by:

\[
ar(r-1)+br+c=0 \quad \text{(1)}
\]

with roots $r_1$ and $r_2$. Then, the general solution of the Euler equation:

\[
ax^2y''+bxy'+cy=0 \quad \text{(2)}
\]

on the interval $(0,\infty)$ can be expressed as follows:

1. If $r_1$ and $r_2$ are distinct real numbers:
\[
y=c_1x^{r_1}+c_2x^{r_2} \quad \text{(3)}
\]

2. If $r_1=r_2$:
\[
y=x^{r_1}(c_1+c_2\ln x) \quad \text{(4)}
\]

3. If $r_1$ and $r_2$ are complex numbers of the form $\lambda\pm i\omega$ with $\omega>0$:
\[
y=x^{\lambda}\left[c_1\cos(\omega\ln x)+ c_2\sin(\omega\ln x)\right] \quad \text{(5)}
\]

Let me know if there's anything else I can help you with!
`````

5. Find the general solution of the given Euler equation on $(0,\infty)$.

* a) $x^2y''-7xy'+7y=0$
* b) $x^2y''+5xy'+4y=0$
* c) $x^2y''-3xy'+13y=0$
* d) $12x^2y''-5xy''+6y=0$
* e) $3x^2y''-xy'+y=0$
* f) $x^2y''+3xy'+5y=0$
* g) $x^2y''-xy'+10y=0$
* h) $2x^2y''+3xy'-y=0$

<font color='Green'><b>Solution</b></font>:

* a) $p(r)=r(r-1)-7r+7=(r-7)(r-1)$

\begin{align*}y=c_1x+c_2x^7.\end{align*}
* b) $p(r)=r(r-1)+5r+4=(r+2)^2$

\begin{align*}y=x^{-2}(c_1+c_2 \ln x).\end{align*}
* c) $p(r)=r(r-1)-3r+13=(r-2)^2+9$

\begin{align*}y=x^2[c_1 \cos (3 \ln x)+c_2 \sin (3 \ln x)].\end{align*}
* d) $p(r)=12r(r-1)-5r+6=(3r-2)(4r-3)$

\begin{align*}y=c_1x^{2/3}+c_2 x^{3/4}.\end{align*}
* e) $p(r)=3r(r-1)-r+1=(r-1)(3r-1)$

\begin{align*}y=c_1x+c_2x^{1/3}.\end{align*}
* f) $p(r)=r(r-1)+3r+5=(r+1)^2+4$

\begin{align*}y={ {1\over x}\left[c_1\cos(2 \ln x)+c_2\sin(2 \ln x\right]}.\end{align*}
* g) $p(r)=r(r-1)-r+10=(r-1)^2+9$

\begin{align*}y=x\left[c_1\cos(3 \ln x)+c_2\sin(3 \ln x)\right].\end{align*}
* h) $p(r)=2r(r-1)+3r-1=(r+1)(2r-1)$

\begin{align*}
y={{c_1\over x}+c_2 x^{1/2}}.
\end{align*}

***
**Refrences**

1. Trench, William F. "Elementary differential equations with boundary value problems." (2018).
***
