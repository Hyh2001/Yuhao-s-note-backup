#probability/continuous_random_variable 

A random variable $Y$ is said to have a beta probability distribution with parameters $\alpha > 0$ and $\beta > 0$ if and only if the density function of $Y$ is  
​$f(y) = {\begin{aligned} \frac{y^{\alpha -1}(1-y)^{\beta -1}}{B(\alpha,\beta)}, 0 \leq y \leq 1 \\ 0, elsewhere \end{aligned}}$  
​$B(\alpha,\beta) = \int_0^1 y^{\alpha -1}(1-y)^{\beta-1} dy = \frac{\gamma(\alpha)\gamma(\beta)}{\gamma(\alpha + \beta)}$         $\gamma( )$ is the Gamma function[^1]

# the [[expected value]] of Beta distribution

$E[Y] = \frac{\alpha}{\alpha + \beta}$

# the [[variance]] of Beta distribution

$\sigma^2 = V[Y] = \frac{\alpha\beta}{(\alpha+\beta)^2(\alpha+\beta+1)}$

‍

‍

1. [probability - Excerpt of: mathematical statistics with applications, p219](lt://open/OxxR2YnPQ0CTGq2QUBqgyQ)