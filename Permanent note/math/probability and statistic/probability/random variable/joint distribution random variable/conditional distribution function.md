# conditional distribution function

Given $Y_1$ and $Y_2$ are random variables with joint density function[^1] or joint probability mass function[^2] $f(x_1,x_2)$, then we can define conditional distribution function as:

$F(y_1|y_2) = P(Y_1 \leq y_1|y_2)$,

​​***for diescrete random variables: ​***

$F(y_1|y_2) = P(Y_1 \leq y_1|y_2) = \sum_{-\infty}^{y_1} \frac{p(y_1,y_2)}{p_2(y_2)}$

***for continuous random variables: ​***

$F(y_1|y_2) = P(Y_1 \leq y_1|y_2) = \int_{-\infty}^{y_1} \frac{p(y_1,y_2)}{p_2(y_2)}$

‍

‍

‍

‍

1. [Project - probability](lt://open/W2ukf6bx8k6Xy9JkM8bylA)

[^1]: # joint density function

    We define it as: if $Y_1$ and $Y_2$ are jointly continuous random variables with a joint desity function given by $f(y_1,y_2)$, then 

    1. $$
        f(y_1,y_2) \geq 0 \quad for \quad all \quad  y_1,y_2
        $$
    2. $$
        \int^{\infty}_{-\infty} \int^{\infty}_{-\infty} f(y_1,y_2)dy_1dy_2 = 1
        $$

    It is just the same of the probability of the intersection of $Y_1$ and $Y_2$: $P(Y_1 \cap Y_2)$  

    ‍

    ‍

    ‍

    ‍

    1. [mathematical statistics with applications - Excerpt of: mathematical statistics with applications, p253](lt://open/-2hfbencnk-4OES8R--fhg)

    2. [probability - Excerpt of: Miller - 2017 - The probability lifesaver all the tools you need , p282](lt://open/h6WnKXWaOEizu9jzvag-Kw)


[^2]: # joint probability mass function

    We define it as: let $Y_1$ and $Y_2$ be discrete random variables. The joint probability function for $Y_1$ and $Y_2$ is as 

    $p(y_1,y_2) = P(Y_1 = y_1, Y_2 = y_2)$ with $-\infty < y_1, y_2 < \infty$ 

    It is just the same of the probability of the intersection of $Y_1$ and $Y_2$: $P(Y_1 \cap Y_2)$ 

    ‍

    1. [mathematical statistics with applications - Excerpt of: mathematical statistics with applications, p250](lt://open/arPPi_R080uMUNOP0yl6SQ)
    2. [Rice_2007_Mathematical statistics and data analysis - Excerpt of: Rice_2007_Mathematical statistics and data analysis, p89](lt://open/uUeVo2pw7kWAL01WbDkwHQ)

    ‍

    ‍
