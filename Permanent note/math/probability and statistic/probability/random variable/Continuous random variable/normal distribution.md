​ #probability/continuous_random_variable #todo 

Normal distribution is also called Gaussian distribution. We say that $X$ is normally distributed with parameters $\mu$ and $\sigma^2$, if the density of $X$ is given that
$f(x) = \frac{1}{\sqrt{2\pi}\sigma}e^{-(x-\mu)^2/2\sigma^2}$    $-\infty < x <\infty$
The property of the distribution is as follow:

1. The density function is symmetric about $\mu$, so $\mu$ determines the shape of the curve.
2. $\sigma$ will control the shape of the curve.

The expected value of a normal distribution is $\mu$ and the variance is $\sigma^2$ 

# normal distribution of functions of a random variable

Let $Y = aX + b$, if $X$ is normally distributed with parameters $\mu$ and $\sigma$, then $Y$ is normally distributed with $a\mu +b$ and $a^2\mu^2$.  To proof this we can see below:

## proof

We denote that the cumulative distribution function of $Y$ is  
$F_Y(x) = P\{ Y \leq x\} = P\{aX + b \leq x\} = P\{X \leq \frac{x-b}{a}\} = F_x(\frac{x-b}{a})$  
Next we differentiate the function and we get  
$f_Y(x) = \frac{1}{a} f_x(\frac{x-b}{a}) = \frac{1}{\sqrt{2\pi}a\sigma}e^{-(x-b-a\mu)^2/2(a\sigma)^2}$

Also, with this property, we can define standard normal distribution[^1].

# normal distribution approximate binomial distribution

Normal distribution can be also used to approximate binomial distribution[^3]. 

When $n$ is large, a Binomial distribution with parameters $n$ and $p$ will have approximately the same distribution as a normal distribution whose mean is $\mu = np$ and standard deviation is $\sigma = \sqrt{np(1-p)}$ This approximation will be quite good if $\sigma^2 = np(1-p) \geq 10$ ​ $^{[1]}$ Or $n > 20$ and $np > 5$ ​ $^{[2]}$  

## continuity correlation 

Because binomial distribution is a discrete random variable and normal distribution is a continuous random variable when calculating boundary conditions, we should add or substract $0.5$. For example: 

1. If we want  to find $P(40\leq X \leq 45)$ in binomial distribution, then, we need to calculate $P(39.5<X< 45.5)$ for normal distribution.
2. If what we want is $P(40 < X < 45)$, then, we need to calculate $P(40.5<X< 44.5)$ for normal distribution.    

    ‍

1. [Normal Approximation to Binomial: Definition &amp; Example (statology.org)](https://www.statology.org/normal-approximation/)

For $^{[1]}$, it is from the book *&quot; the first class in probability&quot;*  
For $^{[2]}$, it is from the book *&quot; mathematical statistic with applications&quot;*

‍



# normal distribution approximate Poisson distribution

If $\lambda \geq 20$ for a Poisson distribution[^6], then we can say that it can be approximated by normal distribution with $\mu = \lambda$ and $\sigma = \sqrt{\mu}$.

## proof:

​ #todo #​    

‍

‍

‍

‍

[Project - probability](lt://open/zk8HC6__90WhHLTFbpQumQ)
