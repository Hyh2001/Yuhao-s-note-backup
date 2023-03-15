---
sr-due: 2023-02-10
sr-interval: 3
sr-ease: 250
---

#probability/continuous_random_variable #review 
Then definition of Gama distribution is as follow.  
A random variable $Y$ is said to have a gamma distribution with parameters $\alpha > 0$ and $\beta > 0$ if and only if the density function of $Y$ is  
​$f(y) = {\begin{aligned}\frac{y^{\alpha-1}e^{-y/\beta}}{\beta ^\alpha \gamma(\alpha)} , y \geq 0 \\ 0 , y < 0 \end{aligned}}$  
​$\gamma(\alpha)$ is the [[Gamma function]].

## real world meaning

This distribution is used to approximate time before some process occurs.

### why? 

​#todo#​ 

‍

# shape of the [[probability density function]]

Most of the area under the density function is located near the origin.  
​![[Pasted image 20221024122116.png]]
## shape parameter ($\alpha$)

The shape of the distribution is determined by the parameter $\alpha$. With $\alpha$ differs, shape differs.

## scale parameter($\beta$)

The scale of the distribution is determined by the parameter $\beta$. With $\beta$ differs, scale differs.

# expected value and variance of Gamma distribution

$E[Y] = \alpha\beta$, $V[Y] = \alpha\beta^2$

### proof

​#todo#​

$E[Y] =

# programming implementation

```excel
# given x,alpha and beta to find probability
GAMMA.DIST(x,alpha,beta,cumulative) 

# given probability, alpha and beta to find x 
GAMMA.INV(probability, alpha, beta)
```

# [[Gamma distribution - Poisson distribution]]



1. #todo 