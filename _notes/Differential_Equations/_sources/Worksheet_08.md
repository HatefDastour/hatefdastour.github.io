# Worksheet 08

1. Find the general solution.

* a).  $y^{(4)}+12y''+36y=0$
* b).  $6y^{(4)}+5y'''+7y''+5y'+y=0$
* c).  $y^{(4)}-4y'''+7y''-6y'+2y=0$

<font color='Green'><b>Solution</b></font>:

* a).
We have $p(r)=r^4+12r^2+36=(r^2+6)^2$, and
\begin{align*}y=(c_1+c_2x)\cos\sqrt{6} x+(c_3+c_4x)\sin\sqrt{6} x.\end{align*}
* b).
Since $p(r)=6r^4+5r^3+7r^2+5r+1=(2r+1)(3r+1)(r^2+1)$,
\begin{align*}y=c_1e^{-x/2}+c_2e^{-x/3}+c_3\cos x+c_4\sin x.\end{align*}
* c).
The characteristic polynomial: $p(r)=r^4-4r^3+7r^2-6r+2=(r-1)^2(r^2-2r+2)$. Then,
\begin{align*}y=e^x(c_1+c_2x+c_3\cos x+c_4\sin x).\end{align*}


***

## Undetermined Coefficients For Higher Order Equations

`````{admonition} Undetermined Coefficients For Higher Order Equations
:class: important
Consider the constant coefficient equation:

\begin{equation}
 \label{eq:9.3.1} a_0y^{(n)}+a_1y^{(n-1)}+\cdots+a_ny=F(x),
\end{equation}

where $n\ge3$ and $F$ is a linear combination of functions of the form:

$$
e^{\alpha x}\left(p_0+p_1x+\cdots+p_kx^k\right)
$$

or

$$
e^{\lambda x}\left[\left(p_0+p_1x+\cdots+p_kx^k\right)\cos(\omega x)+\left(q_0+q_1x+\cdots+q_kx^k\right)\sin(\omega x)\right].
$$

According to Theorem 9.1.5, the general solution of equation \eqref{eq:9.3.1} is given by $y=y_p+y_c$, where $y_p$ is a particular solution of equation \eqref{eq:9.3.1} and $y_c$ is the general solution of the complementary equation:

$$
a_0y^{(n)}+a_1y^{(n-1)}+\cdots+a_ny=0.
$$
`````



2. First, find a particular solution for \begin{align*}y''-4y'+4y=2+8x-4x^2.\end{align*} Then, find the general solution for the given ODE.
    
<font color='Green'><b>Solution</b></font>:

The characteristic polynomial of the complementary equation:
\begin{align*}p(r)=r^2-4r+4=(r-2)^2.\end{align*}

a fundamental set of solutions for the complementary equation:
\begin{align*}\{e^{2x},xe^{2x}\}.\end{align*}

To find a particular solution, we can use the method of undetermined coefficients. let $y_p=A+Bx+Cx^2$; then
\begin{align*}
y_p''-4y_p'+4y_p&=2C-4(B+2Cx)+4(A+Bx+Cx^2)\\
&=(2C-4B+4A)+(-8C+4B)x+4Cx^2,
\end{align*}
and
\begin{align*}(2C-4B+4A)+(-8C+4B)x+4Cx^2=2+8x-4x^2.\end{align*}
Therefore, $4C=-4,\ -8C+4B=8,\ 2C-4B+4A=2$, so $C=-1$, $B=0$, and $A=1$.
Therefore, $y_p=1-x^2$ is a particular solution and
 $y=1-x^2+e^{2x}(c_1+c_2x)$ is the general solution.

***

3. Find a particular solution.
* a). $y'''-2y''-5y'+6y=e^{-3x}(32-23x+6x^2)$,
* b). $y'''+3y''-y'-3y=e^{-2x}(2-17x+3x^2)$,
* c). $y'''+y''-2y=e^x(14+34x+15x^2)$,
* d). $y^{(4)}-3y'''+2y''+2y'-4y=e^x(2\cos2x -\sin2x)$.

<font color='Green'><b>Solution</b></font>:
* a). 
If $y=ue^{-3x}$, then
\begin{align*}
y'''-2y''-5y'+6y&=e^{-3x}[(u'''-11u''+34u'-24u)-2(u''-6u'+9u)-5(u'-3u)+6u]\\
&=e^{-3x}(u'''-11u''+34u'-24u).
\end{align*}
Thus,
\begin{align*}
e^{-3x}(u'''-11u''+34u'-24u) = e^{-3x}(32-23x+6x^2)$,
\end{align*}
or
\begin{align*}
u'''-11u''+34u'-24u = 32-23x+6x^2$,
\end{align*}
Since the unknown $u$ appears on the left, we can see that has a particular solution of the form
\begin{align*}u_p=A+Bx+Cx^2.\end{align*}
Then,
\begin{align*}(-24A+34B-22C)+(-24B+68C)x-24Cx^2=32-23x+6x^2.\end{align*}
It follows that $A=-3/4$, $B=1/4$, and $C=-1/4$. Therefore,
\begin{align*}y_p=-\dfrac{e^{-3x}}{4}(3-x+x^2).\end{align*}

* b). Similarly, let $y=ue^{-2x}$, then
\begin{align*}
y'''+3y''-y'-3y&=e^{-2x}[(u'''-6u''+12u'-8u)+ 3(u''-4u'+4u) -(u'-2u) -3u]\\
&=e^{-2x}(u'''-3u''-u'+3u).
\end{align*}
and
\begin{align*}
u'''-3u''-u'+3u =2-17x+3x^2).
\end{align*}
Now, let $u_p=A+Bx+Cx^2$, where $(3A-B-6C)+
(3B-2C)x +3Cx^2=2-17x+3x^2$.
It can be seen that $A=1$, $B=-5$, and $C=1$. Hence,
\begin{align*}y_p=e^{-2x}(1-5x+x^2).\end{align*}

* c). 
Let $y=ue^x$, then
\begin{align*}
y'''+y''-2y & =e^x[(u'''+3u''+3u'+u) +(u''+2u'+u) -2u]\\
&= e^x(u'''+4u''+5u').
\end{align*}
It follows that,
\begin{align*}
u'''+4u''+5u'= 14+34x+15x^2.
\end{align*}
Thus, we can find a particular solution of the form
\begin{align*}u_p=x(A+Bx+Cx^2).\end{align*}
We have,
\begin{align*}(5A+8B+6C) +(10B+24C)x +15Cx^2 =14+34x+15x^2.\end{align*}
It follows that, $A=0$, $B=1$, and $C=1$
\begin{align*}y_p=x^2e^x(1+x).\end{align*}

* d). 
Let $y=ue^x$, and then
\begin{align*}
y^{(4)}-3y'''+2y''+2y'-4y&=e^x[(u^{(4)}+4u'''+6u''+4u'+u) -3(u'''+3u''+3u'+u)
\\ & +2(u''+2u'+u) +4(u'+u)+u]\\
&=e^x(u^{(4)}+u'''-u''+u'-2u).
\end{align*}
Thus,
\begin{align*}
u^{(4)}+u'''-u''+u'-2u = 14+34x+15x^2
\end{align*}
Thus, we can find a particular solution of the form
\begin{align*}u_p=A\cos2x+B\sin2x.\end{align*}
where
\begin{align*}
\begin{cases}18A-6B=2,\\6A+18B=-1.\end{cases}
\end{align*}
Thus, $A=1/12$, $B=-1/12$, and
\begin{align*}y_p={e^x\over12}(\cos2x-\sin2x).\end{align*}
***

## Variation Of Parameters for Higher Order Equations

4. Find a particular solution, given the fundamental set of solutions of the complementary equation.
* a). $y'''+6xy''+(6+12x^2)y'+(12x+8x^3)y=x^{1/2}e^{-x^2}$, 
 $\{e^{-x^2},\,xe^{-x^2},\,x^2e^{-x^2}\}$,
* b). $16x^4y^{(4)}+96x^3y'''+72x^2y''-24xy'+9y=96x^{5/2}$, 
$\{\sqrt x,\,1/\sqrt x,\,x^{3/2},\,x^{-3/2}\}$.
    
<font color='Green'><b>Solution</b></font>:

* a). First off,
\begin{equation*}
W=\left|\begin{array}{cccc}
e^{-x^2}&xe^{-x^2}&x^2e^{-x^2}\\
-2xe^{-x^2}&e^{-x^2}(1-2x^2)&2x
e^{-x^2}(1-x^2)\\
e^{-x^2}(4x^2-2)&2xe^{-x^2}(2x^2-3)&2e^{-x^2}(2x^4-5x^2+1)
\end{array}\right|=2e^{-3x^2}.
\end{equation*}
Moreover,
\begin{align*}
W_1&=\left|\begin{array}{cccc}
xe^{-x^2}&x^2e^{-x^2}\\
e^{-x^2}(1-2x^2)&2xe^{-x^2}(1-x^2)
\end{array}\right|=x^2e^{-2x^2},\\
W_2&=\left|\begin{array}{cccc}
e^{-x^2}&x^2e^{-x^2}\\
-2xe^{-x^2}&2xe^{-x^2}(1-x^2)
\end{array}\right|=2xe^{-2x^2},\\
W_3&=\left|\begin{array}{cccc}
e^{-x^2}&xe^{-x^2}\\
-2xe^{-x^2}&e^{-x^2}(1-2x^2)
\end{array}\right|=e^{-2x^2}.
\end{align*}
Therefore,
\begin{align*}
\begin{cases}
u_1'={FW_1\over P_0W}= {1\over2}x^{5/2},\\
u_2'=-{FW_2\over P_0W}= -x^{3/2},\\
u_3'={FW_2\over P_0W}= \sqrt{x}/2.
\end{cases}
\quad \Rightarrow \quad
\begin{cases}
u_1= x^{7/2}/7,\\
u_2= -{2\over5}x^{5/2},\\
u_3= x^{3/2}/3.
\end{cases}
\end{align*}
Thus,
\begin{align*}y_p=u_1y_1+u_2y_2+u_3y_3= {8\over105}e^{-x^2}x^{7/2}.\end{align*}

* b). 
First off,
\begin{equation*}
W=\left|\begin{array}{cccc}
\sqrt{x}&1/\sqrt{x}&x^{3/2}&{1\over x^{3/2}}
\\{1\over
2\sqrt{x}}&-{1\over 2x^{3/2}}&{3\sqrt{x}\over
2}&-{3\over 2x^{5/2}}\\
-{1\over
4x^{3/2}}&{3\over 4x^{5/2}}&{3\over
4\sqrt{x}}&{15\over 4x^{7/2}}\\
{3\over
8x^{5/2}}&-{15\over
8x^{7/2}}&-{3\over 8x^{3/2}}&-{105\over 8x^{9/2}}
\end{array}\right|={12\over x^6}
\end{equation*}
Moreover,
\begin{align*}
&W_1 =
\left|\begin{array}{cccc}
{1\over \sqrt{x}}&x^{3/2}&{1\over x^{3/2}}\\
-{1\over 2x^{3/2}}&{3\sqrt{x}\over 2}&-{3\over
2x^{5/2}}\\
{3\over 4x^{5/2}}&{3\over 4\sqrt{x}}&{15\over 4x^{7/2}}
\end{array}\right|={6\over x^{7/2}},
&W_2=\left|\begin{array}{cccc}
\sqrt{x}&x^{3/2}&{1\over x^{3/2}}\\
{1\over 2\sqrt{x}}&{3\sqrt{x}\over 2}&-{3\over
2x^{5/2}}\\
-{1\over 4x^{3/2}}&{3\over 4\sqrt{x}}&{15\over 4x^{7/2}}
\end{array}\right|={6\over x^{5/2}},
\\
&W_3=\left|\begin{array}{cccc}
\sqrt{x}&{1\over \sqrt{x}}&{1\over x^{3/2}}\\
{1\over 2\sqrt{x}}&-{1\over 2x^{3/2}}&-{3\over
2x^{5/2}}\\
-{1\over 4x^{3/2}}&{3\over 4x^{5/2}}&{15\over 4x^{7/2}}
\end{array}\right|=-{2\over x^{9/2}},
&W_4=\left|\begin{array}{cccc}
\sqrt{x}&{1\over \sqrt{x}}&x^{3/2}\\
{1\over 2\sqrt{x}}&-{1\over 2x^{3/2}}&{3\sqrt{x}\over 2}\\
-{1\over 4x^{3/2}}&{3\over 4x^{5/2}}&{3\over 4\sqrt{x}}
\end{array}\right|=-{2\over x^{3/2}}
\end{align*}
Hence,
\begin{align*}
\begin{cases}
u_1'=-{FW_1\over P_0W}=-3x,\\
u_2'={FW_2\over P_0W}=3x^2,\\
u_3'=-{FW_2\over P_0W}=1,\\
u_4'={FW_4\over P_0W}=-x^3.
\end{cases}
\quad \Rightarrow \quad
\begin{cases}
u_1=-{3x^2\over 2},\\
u_2= x^3,\\
u_3= x,\\
u_4=-{x^4\over 4}.
\end{cases}
\end{align*}
Therefore,
\begin{align*}y_p=u_1y_1+u_2y_2+u_3y_3= {x^{5/2}\over 4}.\end{align*}
***

***
## Refrences
1. Trench, William F. "Elementary differential equations with boundary value problems." (2018).
***
