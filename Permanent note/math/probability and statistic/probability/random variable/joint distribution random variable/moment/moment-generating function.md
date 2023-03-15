 #probability 

The moment generating function is defined as $m_U(t) = E(e^{tU})$. where $U$ is a function $n$ random variables. 

# why we define this function

1. If $m_X(t)$ an $m_Y(t)$ denote he moment-generating function of random variables $X$ and $Y$. If there exist $m_X(t) = m_Y(t)$ for all values of $t$, then $X$ and $Y$ have the same probability distribution.
2. We can use moment-generating equation to calculate moment[^1]more easily: 

    $E[X^n] = \frac{d^n(M_x(t))}{dt^n}|_{t=0}$  

    proof: We can proof the equation above by using the Maclaurin series expansion.  $e^{tX} = 1 + tX + \frac{t^2X^2}{2!} + \frac{t^3X^3}{3!} + ....$ Therefore, $E[e^{tX}] = E[1] + E[tX] + E[\frac{t^2X^2}{2!} ] + E[\frac{t^3X^3}{3!}]....$

# properties of moment-generating functions  

1. If $U = Y_1 + Y_2 +... + Y_n$ and each of then are independent, then $m_U(t) = m_{Y_1}(t) \times m_{Y_2}(t) \times ... \times m_{Y_n}(t)$

    proof: $m_U(t) = E(e^{tU}) = E(e^{t(Y_1 + Y_2 +... + Y_n)}) = E(e^{tY_1}e^{tY_2}...e^{tY_n}) = E(e^{tY_1})\times E(e^{tY_2}) \times ... \times E(e^{tY_n})$

‍

‍

‍

1. [Moments and Moment Generating Functions of Statistical Distributions | by Egor Howell | Towards Data Science](https://towardsdatascience.com/moments-and-moment-generating-functions-of-statistical-distributions-e216cb11a079)
