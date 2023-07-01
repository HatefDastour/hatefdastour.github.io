# Worksheet 10

\begin{align*}
\begin{array}{|ccc|ccc|}
\hline
f(t)                      & F(s)                                                  &            & f(t)                                         & F(s)                                                                        &                  \\ \hline
1                               & \dfrac{1}{s}                                & (s > 0)      & t \sin \omega t                                  & \dfrac{2\omega s}{(s^2+\omega^2)^2}                              & (s>0)              \\
t^n, n \in \mathbb{Z}       & \dfrac{n!}{s^{n+1}}                          & (s > 0)      & \sin \omega t -\omega t\cos  \omega t            & \dfrac{2\omega^3}{ (s^2+\omega^2)^2}                               & (s>0)              \\
t^p,\;  p > -1                & \dfrac{\Gamma (p+1) }{ s^{(p+1)}}             & (s>0)        & \omega t - \sin  \omega t                        & \dfrac{\omega^3 }{ s^2(s^2+\omega^2)^2}                             & (s>0)              \\
e^{at}                        & \dfrac{1 }{s-a}                               & (s > a)      & \dfrac{1 }{ t} \sin  \omega t       & \arctan \left( \dfrac{\omega }{ s}\right)                            & (s>0)              \\
t^ne^{at}, n \in \mathbb{Z} & \dfrac{n! }{(s-a)^{n+1}}                      & (s > 0)      & e^{at}f(t)                                       & F(s-a)                                                                          &                      \\
\cos \omega t                 & \dfrac{s }{ s^2+\omega^2}                     & (s > 0)      & t^kf(t)                                          & (-1)^kF^{(k)}(s)                                              &                      \\
\sin \omega t                 & \dfrac{\omega }{ s^2+\omega^2}                & (s > 0)      & f(\omega t)                                      & \dfrac{1}{\omega} F\left(\dfrac{s }{ \omega}\right),  \quad \omega > 0 &                      \\
e^{\lambda t} \cos \omega t   & \dfrac{s - \lambda }{ (s-\lambda)^2+\omega^2} & (s >\lambda) & u(t-\tau)                                        & \dfrac{e^{-\tau s}}{ s}                                            & (s>0)              \\
e^{\lambda t} \sin \omega t   & \dfrac{\omega }{ (s-\lambda)^2+\omega^2}      & (s >\lambda) & u(t-\tau)f(t-\tau)\, (\tau > 0)                  & e^{-\tau s}F(s)                                                                 &                      \\
\cosh bt                      & \dfrac{s }{s^2-b^2}                          & (s > |b|)    & \int^t_o f(\tau)g(t-\tau)\, d\tau & F(s) \cdot G(s)                                                                 &                      \\
\sinh bt                      & \dfrac{b }{s^2-b^2}                          & (s > |b|)    & \delta(t-a)                                      & e^{-as}                                                                         & (s>0)              \\
t \cos \omega t               & \dfrac{s^2-\omega^2 }{ (s^2+\omega^2)^2}      & (s>0)      & & &\\ \hline
\end{array}
\end{align*}

1. Use  the table of Laplace transforms to find the Laplace transforms of the following functions.

* a) $\cosh t\sin t$,
* b) $\sin^2t$,
* c) $\cos^2 2t$,
* d)  $\cosh^2 t$,
* e) $t\sinh 2t$,
* f) $\sin t\cos t$,
* g) $\sin\left(t+{\pi/4}\right)$,
* h) $\cos 2t -\cos 3t$,
* i) $\sin 2t +\cos 4t$.

<font color='Green'><b>Solution</b></font>:

* a)
$
\cosh t\sin t=\displaystyle{{1\over
2}\left(e^t\sin t+e^{-t}\sin t\right)}
\leftrightarrow
\displaystyle{{1\over2}\left[{1\over(s-1)^2+1}+{1\over(s+1)^2+1}\right]}
=\displaystyle{s^2+2\over[(s-1)^2+1][(s+1)^2+1]}.
$

* b)
$\displaystyle
\sin^2t={1-\cos2t\over2}\leftrightarrow{1\over2}\left[{1\over s}
-{s\over(s^2+4)}\right]={2\over s(s^2+4)}$.

* c)
$\displaystyle \cos^22t={1\over2}\left[{1\over s}+{s\over
s^2+16}\right]=
{s^2+8\over s(s^2+16)}$.

* d)
$\cosh^2
t=\displaystyle{(e^t+e^{-t})^2)\over4}=\displaystyle{(e^{2t}+2+e^{-2t})\over4}
\leftrightarrow\displaystyle{{1\over4}\left({1\over s-2}+{2\over s}+{1\over
s+2}\right)} =\displaystyle{s^2-2\over s(s^2-4)}$.

* e)
$t\sinh2t=\displaystyle{te^{2t}-te^{-2t}\over2}
\leftrightarrow\displaystyle{{1\over2}\left({1\over(s-2)^2}-{1\over(s+2)^2}\right)}
=\displaystyle{4s\over(s^2-4)^2}$.

* f)
$\displaystyle\sin t\cos t={\sin2t\over2}\leftrightarrow{1\over
s^2+4}$.

* g)
$\displaystyle\sin(t+\pi/4)=\sin
t\cos(\pi/4)+\cos
t\cos(\pi/4)\leftrightarrow{1\over\sqrt{2}}\,{s+1\over s^2+1}$.

* h)
$\cos 2t -\cos 3t\leftrightarrow\displaystyle{s\over
s^2+4}-\displaystyle{s\over s^2+9}=\displaystyle{5s\over(s^2+4)(s^2+9)}$.

* i)
 $\sin 2t +\cos4t\leftrightarrow\displaystyle{2\over
s^2+4}+\displaystyle{s\over s^2+16} =\displaystyle{s^3+2s^2+4s+32\over(s^2+4)(s^2+16)}$.
***

2. Find the inverse Laplace transform of the following functions.

* a) $\dfrac{2s+3}{(s-7)^4}$
* b) $\dfrac{s^2-1}{(s-2)^6}$
* c) $\dfrac{s+5}{ s^2+6s+18}$
* d) $\dfrac{2s+1}{ s^2+9}$
* e) $\dfrac{s}{ s^2+2s+1}$
* f) $\dfrac{s+1}{ s^2-9}$
* g) $\dfrac{s^3+2s^2-s-3}{(s+1)^4}$
* h) $\dfrac{2s+3}{(s-1)^2+4}$
* i) $\dfrac{1}{ s}-\dfrac{s}{ s^2+1}$
* j) $\dfrac{3s+4}{ s^2-1}$
* k) $\dfrac{3}{ s-1}+\dfrac{4s+1}{ s^2+9}$
* l) $\dfrac{3}{(s+2)^2}-\dfrac{2s+6}{ s^2+4}$

<font color='Green'><b>Solution</b></font>:

* a)
Note that
\begin{align*}
\displaystyle{2s+3\over(s-7)^4}&=\displaystyle{2(s-7)+17\over(s-7)^4}=
\displaystyle{2\over(s-7)^3}+{17\over(s-7)^4}
\\ 
\displaystyle{2s+3\over(s-7)^4}&=\displaystyle{2!\over(s-7)^3}+\displaystyle{17\over6}{3!\over(s-7)^4}
\leftrightarrow e^{7t}\displaystyle{\left(t^2+{17\over6}t^3\right)}
\end{align*}

* b)
\begin{align*}
\displaystyle{s^2-1\over(s-2)^6}&=\displaystyle{[(s-2)+2]^2-1\over(s-2)^6}
=\displaystyle{(s-2)^2+4(s-2)+3\over(s-2)^6}
=\displaystyle{1\over(s-2)^4}+\displaystyle{4\over(s-2)^5}+\displaystyle{3\over(s-2)^6}
\\ 
\displaystyle{s^2-1\over(s-2)^6}&=\displaystyle{{1\over6}{3!\over(s-2)^4}}+\displaystyle{{1\over6}{4!\over(s-2)^5}}
+\displaystyle{{1\over40} {5!\over(s-2)^6}}\leftrightarrow\displaystyle{\left({1\over
6}t^3+{1\over6}t^4+{1\over40}t^5\right)e^{2t}}.
\end{align*}

* c)
$\displaystyle{s+5\over s^2+6s+18}={(s+3)\over(s+3)^2+9}
+{2\over3}{3\over(s+3)^2+9}
\leftrightarrow e^{-3t}\left(\cos 3t+{2\over3}\sin 3t\right)$.

* d)
$\displaystyle{2s+1\over s^2+9}=2{s\over
s^2+9}+{1\over3}{3\over s^2+9}\leftrightarrow
\displaystyle{2\cos 3t+{1\over3}\sin 3t}$.

* e)
$\displaystyle{s\over s^2+2s+1}={(s+1)-1\over(s+1)^2}=
{1\over s+1}-{1\over (s+1)^2}\leftrightarrow
(1-t)e{^{-t}}$.

* f)
$\displaystyle{s+1\over s^2-9}={s\over s^2-9}+{1\over3}{3\over
s^2-9}\leftrightarrow {\cosh 3t+{1\over3}\sinh 3t}$.

* g)
Expand the numerator in powers of $s+1$:
\begin{align*}
s^3+2s^2-s-3&=[(s+1)-1]^3+2[(s+1)-1]^2-[(s+1)-1]-3
\\&
=(s+1)^3-(s+1)^2-2(s+1)-1.
\end{align*}
Therefore,
\begin{align*}\displaystyle{s^3+2s^2-s-3\over(s+1)^4}={1\over s+1}-{1\over(s+1)^2}
-{2\over(s+1)^3}-{1\over6}{6\over(s+1)^4}\leftrightarrow
{\left(1-t-t^2-{1\over6}t^3\right)e^{-t}}.\end{align*}

* h)
$\displaystyle{2s+3\over(s-1)^2+4}=2{(s-1)\over(s-1)^2+4}
+{5\over2}{2\over(s-1)^2+4}\leftrightarrow
{e^t\left(2\cos 2t+{5\over2}\sin 2t\right)}$.

* i)
$\displaystyle{1\over s}-{s\over s^2+1}\leftrightarrow 1-\cos t$.

* j)
$\displaystyle{3s+4\over s^2-1}=\displaystyle{3s\over s^2-1}+{4\over s^2-1}
\leftrightarrow3\cosh t+4\sinh t.$
Alternatively,
\begin{align*}\displaystyle{3s+4\over
s^2-1}=\displaystyle{3s+4\over(s-1)(s+1)}=\displaystyle{{1\over2}\left[{7\over
s-1}-{1\over s+1}\right]}
\leftrightarrow\displaystyle{7e^t-e^{-t}\over2}.\end{align*}

* k)
$\displaystyle{3\over s-1}+{4s+1\over s^2+9}=3{1\over s-1}
+4{s\over s^2+9}+{1\over3}{3\over s^2+9}\leftrightarrow
\displaystyle{3e^t+4\cos 3t+{1\over3}\sin 3t}$.

* l)
$\displaystyle{3\over(s+2)^2}-{2s+6\over s^2+4}=
3{1\over(s+2)^2}-2{s\over s^2+4}-3{2\over s^2+4}\leftrightarrow
3te^{-2t}-2\cos 2t-3\sin 2t$.
***

3. Find the inverse Laplace transform.
* a) $\displaystyle{2+3s\over(s^2+1)(s+2)(s+1)}$
* b) $\displaystyle{3s^2+2s+1\over(s^2+1)(s^2+2s+2)}$
* c) $\displaystyle{3s+2\over(s-2)(s^2+2s+5)}$
* d) $\displaystyle{3s^2+2s+1\over(s-1)^2(s+2)(s+3)}$
* e) $\displaystyle{2s^2+s+3\over(s-1)^2(s+2)^2}$
* f) $\displaystyle{3s+2\over(s^2+1)(s-1)^2}$

<font color='Green'><b>Solution</b></font>:

* a)
\begin{align*}
{2+3s\over(s^2+1)(s+2)(s+1)}=
{A\over s+2}+{B\over s+1}+{Cs+D\over s^2+1},
\end{align*}
where
\begin{align*}
A(s^2+1)(s+1)+
B(s^2+1)(s+2)+(Cs+D)(s+2)(s+1)=2+3s.
\end{align*}
\begin{align*}
\begin{array}{rcrl}
-5A&=&-4&(\mbox{set }s=-2);\\
2B&=&-1& (\mbox{set }s=-1);\\
A+2B+2D&=&2&(\mbox{set }s=0);\\
A+B+C&=&0&(\mbox{equate coefficients of }s^3).
\end{array}
\end{align*}
Solving this system yields $A=\displaystyle{4\over5}$, $B=-\displaystyle{1\over2}$,
$C=-\displaystyle{3\over10}$, $D=\displaystyle{11\over10}$. Therefore,
\begin{eqnarray*}
{2+3s\over(s^2+1)(s+2)(s+1)}&=&
{4\over5}{1\over s+2}-{1\over2}{1\over s+1}-{1\over10}{3s-11\over
s^2+1}\\
{2+3s\over(s^2+1)(s+2)(s+1)}&\leftrightarrow&
{4\over5}e^{-2t}-{1\over2}e^{-t}-{3\over10}\cos t
+{11\over10}\sin t.
\end{eqnarray*}

* b)
\begin{align*}
{3s^2+2s+1\over(s^2+1)(s^2+2s+2)}=
{As+B\over s^2+1}+{C(s+1)+D\over(s+1)^2+1},
\end{align*}
where
\begin{align*}
(As+B)((s+1)^2+1)+(C(s+1)+D)(s^2+1)=3s^2+2s+1.
\end{align*}
\begin{align*}
\begin{array}{rcrl}
2B+C+D&=&1&(\mbox{set }s=0);\\
-A+B+2D&=&2& (\mbox{set }s=-1);\\
2B+C+D&=&1&(\mbox{set }s=0);\\
A+C&=&0&(\mbox{equate coefficients of }s^3).
\end{array}
\end{align*}
Solving this system yields
$A=6/5$, $B=2/5$, $C=-6/5$, $D=7/5$.
Therefore,
\begin{eqnarray*}
{3s^2+2s+1\over(s^2+1)(s^2+2s+2)}&=&
{1\over5}\left[{6s+2\over s^2+1}-{6(s+1)-7\over(s+1)^2+1}\right]\\
{3s^2+2s+1\over(s^2+1)(s^2+2s+2)}&\leftrightarrow&
 {6\over5}\cos t+{2\over5}\sin t
-{6\over5}e^{-t}\cos t+{7\over5}e^{-t}\sin t.
\end{eqnarray*}

* c)
$s^2+2s+5=(s+1)^2+4$;
\begin{align*}
{3s+2\over(s-2)((s+1)^2+4)}={A\over s-2}+
{B(s+1)+C\over(s+1)^2+4},
\end{align*}
where
\begin{align*}
A\left((s+1)^2)+4\right)+
\left(B(s+1)+C\right)(s-2)=3s+2.
\end{align*}
\begin{align*}
\begin{array}{rcrl}
13A&=&8&(\mbox{set }s=2);\\
4A-3C&=&-1&(\mbox{set }s=-1);\\
A+B&=&0&(\mbox{equate coefficients of }s^2).
\end{array}
\end{align*}
Solving this system yields $A=\displaystyle{8\over13}$, $B=-\displaystyle{8\over13}$,
$C=\displaystyle{15\over13}$. Therefore,
\begin{eqnarray*}
{3s+2\over(s-2)((s+1)^2+4)}&=&{1\over13}\left[{8\over
s-2}-
{8(s-1)-15\over(s+1)^2+4}\right]\\
{3s+2\over(s-2)((s+1)^2+4)}&\leftrightarrow&
{8\over13}e^{2t}-{8\over13}e^{-t}\cos 2t+{15\over26}
e^{-t}\sin 2t.
\end{eqnarray*}

* d)
\begin{align*}
{3s^2+2s+1\over(s-1)^2(s+2)(s+3)}=
{A\over s-1}+{B\over(s-1)^2}+{C\over s+2}+{D\over s+3},
\end{align*}
where
\begin{align*}
(A(s-1)+B)(s+2)(s+3)+(C(s+3)+D(s+2))(s-1)^2=3s^2+2s+1.
\end{align*}
\begin{align*}
\begin{array}{rcrl}
12B&=&6&(\mbox{set }s=1);\\
9C&=&9& (\mbox{set }s=-2);\\
-16D&=&22&(\mbox{set }s=-3);\\
A+C+D&=&0&(\mbox{equate coefficients of }s^3).
\end{array}
\end{align*}
Solving this system yields
$A=3/8$, $B=1/2$, $C=1$, $D=-11/8$.
Therefore,
\begin{eqnarray*}
{3s^2+2s+1\over(s-1)^2(s+2)(s+3)}&=&
{3\over8}{1\over s-1}+{1\over2}{1\over(s-1)^2}+{1\over
s+2}-{11\over8}{1\over s+3}\\
{3s^2+2s+1\over(s-1)^2(s+2)(s+3)}&\leftrightarrow&
{3\over8}e^t+{1\over2}te^t+e^{-2t}-{11\over8}e^{-3t}.
\end{eqnarray*}

* e)
\begin{align*}
{2s^2+s+3\over(s-1)^2(s+2)^2}=
{A\over s-1}+{B\over(s-1)^2}+{C\over s+2}+{D\over(s+2)^2},
\end{align*}
where
\begin{align*}
(A(s-1)+B)(s+2)^2+(C(s+2)+D)(s-1)^2=2s^2+s+3.
\end{align*}
\begin{align*}
\begin{array}{rcrl}
9B&=&6&(\mbox{set }s=1);\\
9D&=&9& (\mbox{set }s=-2);\\
-4A+4B+2C+D&=&3&(\mbox{set }s=0);\\
A+C&=&0&(\mbox{equate coefficients of }s^3).
\end{array}
\end{align*}
Solving this system yields
$A=1/9$, $B=2/3$, $C=-1/9$, $D=1$.
Therefore,
\begin{eqnarray*}
{2s^2+s+3\over(s-1)^2(s+2)^2}&=&
{1\over9}{1\over s-1}+{2\over3}{1\over(s-1)^2}-{1\over9}{1\over
s+2}+{1\over(s+2)^2}\\
{2s^2+s+3\over(s-1)^2(s+2)^2}&\leftrightarrow&
{1\over9}e^t+{2\over3}te^t-{1\over9}e^{-2t}+te^{-2t}.
\end{eqnarray*}

* f)
\begin{align*}
{3s+2\over(s^2+1)(s-1)^2}={A\over s-1}+{B\over(s-1)^2}+
{Cs+D\over s^2+1},
\end{align*}
where
\begin{align*}
A(s-1)(s^2+1)+B(s^2+1)+(Cs+D)(s-1)^2=3s+2.
\qquad (I)
\end{align*}
Setting $s=1$ yields $2B=5$, so $B=\displaystyle{5\over2}$.
Substituting this into (I) shows that
\begin{eqnarray*}
A(s-1)(s^2+1)+(Cs+D)(s-1)^2&=&3s+2-{5\over2}(s^2+1)\\
&=&-{5s^2-6s+1\over2}=-{(s-1)(5s-1)\over2}.
\end{eqnarray*}
Therefore,
\begin{align*}
A(s^2+1)+(Cs+D)(s-1)={1-5s\over2}.
\end{align*}
\begin{align*}
\begin{array}{rcrl}
2A&=&-2&(\mbox{set }s=1);\\
A-D&=&1/2&(\mbox{set }s=0);\\
A+C&=&0&(\mbox{equate coefficients of }s^2).
\end{array}
\end{align*}
Solving this system yields $A=-1$, $C=1$,
$D=-\displaystyle{3\over2}$. Therefore,
\begin{eqnarray*}
{3s+2\over(s^2+1)(s-1)^2}&=&-{1\over s-1}+{5\over2}{1\over(s-1)^2}
+{s-3/2\over s^2+1}\\
{3s+2\over(s^2+1)(s-1)^2}&\leftrightarrow&
-e^t+{5\over2}te^t+\cos t-{3\over2}\sin t.
\end{eqnarray*}
***

4. Use the Laplace transform to solve the initial value problem.
* a) $y''-y'-6y=2, \quad  y(0)=1,\quad y'(0)=0$,
* b) $y''-4y=2 e^{3t}, \quad  y(0)=1,\quad y'(0)=-1$.


<font color='Green'><b>Solution</b></font>:

* a)
\begin{align*}
(s^2-s-6)Y(s)={2\over s}+s-1={2+s(s-1)\over s}.
\end{align*}
Since $(s^2-s-6)=(s-3)(s+2)$,
\begin{align*}
Y(s)={2+s(s-1)\over s(s-3)(s+2)}
=-{1\over3s}+{8\over15}{1\over s-3}+{4\over5}{1\over
s+2}
\end{align*}
and $y=-\displaystyle{1\over3}+\displaystyle{8\over15}e^{3t}+\displaystyle{4\over5}e^{-2t}$.

* b)
\begin{align*}(s^2-4)Y(s)={2\over s-3}+(-1+s)={2+(s-1)(s-3)\over s-3}.\end{align*}
Since $s^2-4=(s-2)(s+2)$,
\begin{align*}Y(s)={2+(s-1)(s-3)\over(s-2)(s+2)(s-3)}=
-{1\over4}{1\over s-2}+{17\over20}{1\over s+2}+{2\over5}{1\over s-3}\end{align*}
and   $y=\displaystyle-{1\over4}e^{2t}+{17\over
20}e^{-2t}+{2\over5}e^{3t}$.

***
**Refrences**

1. Trench, William F. "Elementary differential equations with boundary value problems." (2018).
***