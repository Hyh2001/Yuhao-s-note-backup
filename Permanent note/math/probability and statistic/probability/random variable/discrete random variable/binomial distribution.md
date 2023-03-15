---
sr-due: 2023-03-14
sr-interval: 10
sr-ease: 210
---

#probability/discrete_random_variable #review #todo 拆分

# Bernoulli trial

## properties

1. For each trial, there are only two possible outcomes, "success" and "fail".
2. For each trial, the probability of success $p$ is constant
3. Repeated Bernoulli trials are independent

# binomial trial

$n$ Bernoulli trials.

## expected value  of Binomial distribution

$E[X] = np$

## variance  of Binomial distribution

$V[X] = np(1-p)$

# multinomial trial

# excel

```excel
BINOM.DIST(number_s,trials,probability_s,cumulative)
```

# approximation of Binomial distribution

We can use several other distribution to approximate binomial distribution. See normal distribution approximate binomial distribution, Poisson distribution approximate binomial distribution

‍