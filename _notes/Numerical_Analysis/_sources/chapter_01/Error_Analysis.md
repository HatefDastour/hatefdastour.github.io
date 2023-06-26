# Error Analysis

A real number such that 123.45 can be represented as
\begin{equation*}
123.45 =  1.10^{2} + 2.10^{1} + 3.10^{0} + 4.10^{-1} + 5.10^{-2}.
\end{equation*}
In this case, 10 is the basis of the decimal system. Computers use base 2 for storing a number which is known as the binary system. For example, for 123.45, we have,
\begin{align*}
123 / 2 &= 61,~R:~1\\
61 / 2 &= 30,~R:~1\\
30 / 2 &= 15,~R:~0\\
15 / 2 &= 7,~R:~1\\
7 / 2 &= 3,~R:~1\\
3 / 2 &= 1,~R:~1\\
1 / 2 &= 0,~R:~1\\
&.\\
0.45 \times 2 &= 0.9 + 0\\
0.9 \times 2 &= 0.8 + 1\\
0.8 \times 2 &= 0.6 + 1\\
0.6 \times 2 &= 0.2 + 1\\
0.2 \times 2 &= 0.4 + 0\\
0.4 \times 2 &= 0.8 + 0\\
0.8 \times 2 &= 0.6 + 1\\
0.6 \times 2 &= 0.2 + 1\\
0.2 \times 2 &= 0.4 + 0\\
0.4 \times 2 &= 0.8 + 0\\
0.8 \times 2 &= 0.6 + 1\\
0.6 \times 2 &= 0.2 + 1
\end{align*}
Thus,
\begin{equation*}
(123.45)_{10} = (1111011.01110011001100110011)_{2}
\end{equation*}
Note that,
\begin{align*}
(1111011.011100110011)_{2} &= (1 \times 2^{6}) + (1 \times 2^{5}) + (1 \times 2^{4}) + (1 \times 2^{3}) + (0 \times 2^{2}) + (1 \times 2^{1})
\\ &
+ (1 \times 2^{0}) + (0 \times 2^{-1}) + (1 \times 2^{-2}) + (1 \times 2^{-3}) + (1 \times 2^{-4}) + (0 \times 2^{-5})
\\ &
+ (0 \times 2^{-6}) + (1 \times 2^{-7}) + (1 \times 2^{-8}) + (0 \times 2^{-9}) + (0 \times 2^{-10})
\\ &
+ (1 \times 2^{-11}) + (1 \times 2^{-12}) = (123.449951171875)_{10}
\end{align*}

## Binary Machine Numbers

In the realm of number storage, a real number is represented using a 64-bit expression. The first bit is allocated for the sign of the number (s). The subsequent 11 bits are designated for the exponent (c), while the remaining 52 bits comprise the binary fraction (f), commonly referred to as the **mantissa**. The following format is employed to showcase each floating-point number.

\begin{equation*}
(-1)^s 2^{c - 1023} (1 + f ).
\end{equation*}

-   $s = 0$, $c = 1$, and $f = 0$ produces the **smallest normalized
    positive number** that can be represented
    $$(-1)^0 2^{1 - 1023} (1 + 0 ) = 2^{- 1022} (1 + 0 )  \approx 0.22251 \times 10^{-307}$$

-   $s = 0$, $c = 2046$, and $f = 1 - 2^{-52}$ produces the **largest
    normalized positive number** that can be represented
    $$(-1)^0 2^{2046 - 1023} (1 + 1 - 2^{-52} ) = 2^{1023} (2 - 2^{-52} )\approx 0.17977 \times 10^{309}$$

-   The **underflow** happens if numbers are smaller than the following
    (in magnitude): $$2^{- 1022} (1 + 0 )$$ The result of underflow is
    usually set to zero!

-   The **overflow** happens if numbers are smaller than the following
    (in magnitude): $$2^{1023} (2 - 2^{-52} )$$ Overflow usually results
    in computations stopping.

## Decimal Machine Numbers

The normalized decimal floating point is in the following form

\begin{equation}
\pm 0.d_{1}d_{2}\ldots d_{k} \times 10^{n},
\end{equation}
where $d_{1}\in \{1,2,\ldots,9\}$ and $d_{1},d_{2},\ldots, d_{k} \in \{0, 1,2,\ldots,9\}$,

Consider the value of $\pi$ as approximately $3.14159265359\ldots$. We have the option to represent this number in a shorter form by using a limited number of significant digits. For instance, we can express it as $3.14$, $3.142$, or $3.1416$. Among these options, the last expression is generally preferred as it displays the four significant digits extracted from the full number.

There are various methods to represent the original number in a concise format with only a few significant digits. One approach is known as chopping, where we simply truncate the remaining digits. For instance, we can approximate $\pi$ as $3.141$ through chopping.

However, a more commonly used technique is rounding. By rounding $\pi = 3.14159265359\ldots$ to three significant digits, we arrive at $3.142$. The rounding process involves adding 1 to the $d_k$ digit if the next digit, $d_{k+1}$, is greater than or equal to 5. Otherwise, we discard the digits beyond $d_k$.

To illustrate, when rounding $\pi$ to three significant digits, the fourth digit is 5, so we add 1 to $d_3$, resulting in $3.142$.

## Absolute and Relative Error
The absolute error is simply the difference between the exact value and the approximation.
\begin{equation}
\text{Absolute Error} = |\text{Exact Value} - \text{Approximation}|
\end{equation}
The relative error is
\begin{equation}
\text{Relative Error} = \dfrac{ |\text{Exact Value} - \text{Approximation}|}{|\text{Exact Value}|}
\end{equation}

The following definition is **Definition 1.16** from
{cite:ps}`burden2005numerical`

`````{admonition} Remark
:class: important

Let $x_{\text{app}}$ be an approximation of $x_{\text{exact}}$ to $t\geq 0$ significant digits. Here, $t$ represents the largest number that satisfies the following equation for a nonnegative integer:

\begin{equation}
\text{Relative Error} = \dfrac{ |x_{\text{app}} - x_{\text{exact}}|}{|x_{\text{exact}}|} \leq 5 \times 10^{-t}.
\end{equation}

`````