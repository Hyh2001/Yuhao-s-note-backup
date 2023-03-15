#probability/joint_distribution_random_variable 

Covariance is used to measure whether two random variables are *linearly ​*dependent or independent. The definition proposed by $^{[1]}$ is that, If $Y_1$ and $Y_2$ are random variables with means $\mu_1$ and $\mu_2$, then covariance is $Cov(Y_1,Y_2) = E[(Y_1 - \mu_1)(Y_2 - \mu_2)]$.

### a quick way to calculate Covariance

$Cov (Y_1, Y_2) = E[(Y_1 - \mu_1)(Y_2 - \mu_2)] = E[Y_1Y_2 - \mu_1Y_2 - \mu_2Y_1 + \mu_1\mu_2] = E(Y_1Y_2) - \mu_1E(Y_2) - \mu_2E(Y_1) + \mu_1\mu_2 = E(Y_1Y_2) - \mu_1\mu_2$  
This prove$^{[2]}$ uses some calculation properties of expected value[^1].

​#todo#​ why covariance can be used to measure dependencies?

# How to measure dependencies?

If $Cov(Y_1,Y_2) = 0$, then independent random variables must be uncorrelated

## proof

For two random variables, if they are independent, their expected value must obey $E[Y_1Y_2] = E[Y_1]E[Y_2]$, thus $Cov = 0$.

If $Cov(Y_1,Y_2) = 1$, then independent random variables must be correlated

# problems faced

In $^{[3]}$ we can see that, we can not directly determine whether two random variables are dependent based on the real value of covariance. Thus we need to define correlation coefficient[^28] to solve this problem.

‍

‍

‍

1. [mathematical statistics with applications - Excerpt of: mathematical statistics with applications, p290](lt://open/ss0djQXkfkCDyK442tBqYw)
2. [mathematical statistics with applications - Excerpt of: mathematical statistics with applications, p291](lt://open/edH080TY-EG2IxJ4jwGo_A)
3. [mathematical statistics with applications - Excerpt of: mathematical statistics with applications, p290](lt://open/T8ulI92hD0OZCnEgkCitFw)
