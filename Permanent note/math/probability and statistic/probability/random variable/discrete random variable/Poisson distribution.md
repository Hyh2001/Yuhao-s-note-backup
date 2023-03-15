#probability/continuous_random_variable 

Poison distribution is a limiting form of binomial distribution. Its probability mass function is like  
$p(i) =  P\{ X = i \} = e^{-\lambda}\frac{\lambda^i}{i!}$ for $i = 0,1,2,...$  

The real world meaning of Poisson distribution is as follow:

1. the probability of obtaining $k$ successes during a given time interval

## expected value of Poisson distribution

$E(x) = \sum xp(x;\lambda) = \lambda$

### proof

$E(x) = \sum \frac{\lambda^x}{(x-1)!}e^{-\lambda} = \lambda\sum \frac{\lambda^{x-1}}{(x-1)!}e^{-\lambda}$

## variance of Poisson distribution

$V(x) = \lambda$

### proof

We can use excel to help us to calculate the value of a poison distribution. The use of excel function is as follow.

# excel

```excel
POISSON.DIST(X,Mean,Cumulative)
```

1. $X$ means the number of  events
2. Mean means the expected value[^1] of events
3. Cumulative is True, then it will calculate the sum of all the events less or equal to $X$. If it is False, then only the probability of $X$ will be given.

# Poisson distribution approximate binomial distribution

Poison distribution is an approximation for a binomial distribution[^3] when $n$ is large and $p$ is small. This can be proved as follow

### proof

let $\lambda = np$ ​ $P\{X = i\} = \frac{n!}{(n-i)!i!} p^i(1-p)^{n-i} = \frac{n!}{(n-i)!i!}(\frac{\lambda}{n})^i (1-\frac{\lambda}{n})^{n-i} = \frac{n(n-1)\cdot \cdot \cdot (n-i+1)}{n^i}\frac{\lambda^i}{i!}\frac{(1-\lambda/n)^n}{(1-\lambda/n)^i}$ For $n$ is very large and $p$ is very small  
$(1-\lambda/n)^n \simeq e^{-\lambda}$  $\frac{n(n-1)\cdot \cdot \cdot (n-i+1)}{n^i} \simeq 1$  $(1-\lambda/n)^i \simeq 1$  
Then we get Poisson distribution. Therefore, a binomial distribution with $n$ trails and probability $p$ can be approximated by a Poisson distribution with $\lambda = np$ 

# Poisson distribution and normal distribution

see normal distribution approximate Poisson distribution[^8]

# Poisson distribution and exponential distribution[^9]

see Exponential distribution and Poisson distribution[^13]

# Poisson distribution and Gamma distribution

Gamma distribution and Poisson distribution[^14]
