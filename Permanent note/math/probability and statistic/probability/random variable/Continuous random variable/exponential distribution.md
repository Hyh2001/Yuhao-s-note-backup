#probability/continuous_random_variable #todo 拆分

The probability density function of exponential distribution is as follow.  
​$f(X) = {\begin{aligned}\lambda e^{-\lambda x} , x \geq 0 \\ 0 , x < 0 \end{aligned}}$  
It is a special form of Gamma distribution[^1] when $\alpha = 1$ and $\lambda = \frac{1}{\beta}$  

It is often arises as the distribution of the amount of time until some specific event occurs.

The expected value of normal distribution is 

$E[X] = \frac{1}{\lambda}$

and the variance of it is 

$V[X] = \frac{1}{\lambda ^2}$  

# programming implementation

```excel
EXPON.DIST(x,lambda,cum)
```

# Exponential distribution and Poisson distribution[^4]

Considering the number of events during a particular period of time  
$p(x;\lambda t) = \frac{(\lambda t)^x}{x!}e^{-\lambda t}$  
where $\lambda$ is the number of Poisson events per unit time and $t$ is the number of time units.  
The ***time between Poisson events*** have the exponential distribution with parameter $\beta = \frac{1}{\lambda}$

## proof 

If we consider a time interval $x$ in which no event occurred, we can have a relationship that 

$P(X_t>x) = P(N_t = N_{t+x})$ where $N_t$ is the number denotes cumulative number of the occurrence of an event during $t$ interval.

Then, $P(X_t \leq x) = 1- P(N_t = N_{t+x})$ which denotes that $P(N_x = 0)$. We use Poisson distribution to model and we get $p(N_x = 0) = \frac{{(\lambda x)}^0}{0!}e^{-\lambda x} = e^{-\lambda x} = 1- P(X_t \leq x)$ where we can get $P(X_t \leq x) = 1- e^{-\lambda x}$. This function is exactly same to the probability cumulative function of an exponential distribution. 
