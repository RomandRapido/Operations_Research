# Lagrange Interpolating Polynomial Problem

## Question
Construct the Lagrange interpolating polynomials for $f(x) = \sin(\ln x)$ given $x_0 = 2.0$, $x_1 = 2.4$, $x_2 = 2.6$, $n = 2$.

## Solution
$f(x_0) = f(2.0) = \sin(\ln(2.0)) =  \approx 0.639$

$f(x_1) = f(2.4) = \sin(\ln(2.4)) = \approx 0.7678$

$f(x_2) = f(2.6) = \sin(\ln(2.6)) \approx 0.8166$

$$
\begin{align}
L_0(x) &= \frac{(x - x_1)(x - x_2)}{(x_0 - x_1)(x_0 - x_2)} \\
&= \frac{(x - 2.4)(x - 2.6)}{(2.0 - 2.4)(2.0 - 2.6)}\\
&=\frac{(x - 2.4)(x - 2.6)}{0.24}
\end{align}
$$

$$
\begin{align}
L_1(x) &=  \frac{(x - x_0)(x - x_2)}{(x_1 - x_0)(x_1 - x_2)} \\
&= \frac{(x - 2.0)(x - 2.6)}{(2.4 - 2.0)(2.4 - 2.6)} \\
&=\frac{(x - 2.0)(x - 2.6)}{-0.08}
\end{align}
$$

$$
\begin{align}
L_2(x) &=  \frac{(x - x_0)(x - x_1)}{(x_2 - x_0)(x_2 - x_1)} \\
&=  \frac{(x - 2.0)(x - 2.4)}{(2.6 - 2.0)(2.6 - 2.4)} \\
&=\frac{(x - 2.0)(x - 2.4)}{0.12}
\end{align}
$$

The complete Lagrange interpolating polynomial is:

$$P(x) = L_0(x) \cdot f(x_0) + L_1(x) \cdot f(x_1) + L_2(x) \cdot f(x_2)$$

$$P(x) = \frac{(x - 2.4)(x - 2.6)}{0.24} \cdot 0.639 + \frac{(x - 2.0)(x - 2.6)}{-0.08} \cdot 0.7678 + \frac{(x - 2.0)(x - 2.4)}{0.12} \cdot 0.8166$$