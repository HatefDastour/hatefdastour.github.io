# Error Analysis

## Binary Machine Numbers

When it comes to storing a number, a 64-bit (binary digit) expression is used for a real number. The bit is dedicated to the sign of a number. The next 11 bits are dedicated to the exponent, and the remaining bits (52 bits) are for the binary fraction. The following form is used for demonstrating each floating number.

\begin{align*}
(-1)^s 2^{c - 1023} (1 + f ).
\end{align*} 


* $s = 0$, $c = 1$, and $f = 0$ produces the smallest normalized positive number that can be represented

\begin{align*}
(-1)^0 2^{1 - 1023} (1 + 0 ) \approx 0.22251 \times 10^{-307}
\end{align*} 


* $s = 0$, $c = 2046$, and $f = 1 - 2^{-52}$ produces the largest normalized positive number that can be represented

\begin{align*}
(-1)^0 2^{20461 - 1023} (1 + 1 - 2^{-52} ) \approx 0.17977 \times 10^{309}
\end{align*} 

* The **underflow** happens if numbers are smaller than the following (in magnitude):
\begin{align*}
(-1)^0 2^{1 - 1023} (1 + 0 ) = 2^{- 1022} (1 + 0 ) \approx 0.22251 \times 10^{-307}
\end{align*} 

* The **overflow** happens if numbers are smaller than the following (in magnitude):
\begin{align*}
(-1)^0 2^{20461 - 1023} (1 + 1 - 2^{-52} ) = 2^{1023} (2 - 2^{-52} ) \approx 0.17977 \times 10^{309}
\end{align*} 

## Decimal Machine Numbers

The normalized decimal floating point is in the following form

\begin{align*}
\pm 0.d_{1}d_{2}\ldots d_{k} \times 10^{n},
\end{align*}
where $d_{1}\in \{1,2,\ldots,9\}$ and $d_{1},d_{2},\ldots, d_{k} \in \{0, 1,2,\ldots,9\}$,

Observe that $\pi = 3.14159265359\ldots$. We can a shorter version of this number, for example, $3.14$, $3.142$, or $3.1416$. The last expression is preferred as it shows the four digits from the full numbers. This set of correct digits is also known as **significant digits**.

There are a few ways to represent the original number in a short form and with a few **significant digits**. One way would be just merely chopping off the remaining digits, for example, $\pi \approx 3.141$. This method is known as chopping. Another way would be **rounding** which is way more popular. For example, $\pi = 3.14159265359\ldots$ can be rounded to $3.142$ with three significant digits.

For rounding, we add 1 to $d_{k}$ if $d_{k+1} \geq 5$; otherwise, chop off after $d_{k}$. For example, rounding $\pi = 3.14159265359\ldots$ to three digits, it would be $3.142$ as the 4th digit is 5 and we simply add 1 to $d_{3}$.

## Absolute and Relative Error

The absolute error is simply the difference between the exact value and the approximation.

\begin{align*}
\text{Absolute Error} = |\text{Exact Value} - \text{Approximation}|
\end{align*}

The relative error is
\begin{align*}
\text{Relative Error} = \frac{ |\text{Exact Value} - \text{Approximation}|}{|\text{Exact Value}|}
\end{align*}

`````{admonition} Remark
:class: tip

The approximation $x_{\text{app}}$ of $x_{\text{exact}}$ to $t\geq 0$ significant digits if $t$ is the largest number that satisfy the following equation 
nonnegative integer for which
\begin{align*}
\text{Absolute Error} = \frac{ |x_{\text{app}} - x_{\text{exact}}|}{|x_{\text{app}}|} \leq 5 x 10^{-t}.
\end{align*}

`````

***
**References:**
1. Burden, Richard L., and J. Douglas Faires. "Numerical analysis 8th ed." Thomson Brooks/Cole (2005).
1. Atkinson, Kendall E. An introduction to numerical analysis. John wiley & sons, 2008.
1. Khoury, Richard, and Douglas Wilhelm Harder. Numerical methods and modelling for engineering. Springer, 2016.
***