#probability/joint_distribution_random_variable ​ #review 

This method is used for finding probability distribution of a random variable without directly calculating its [[probability density function]]. The method is as follow. 

# discrete type

We are given a probability density function $f_Y(Y)$ of a discrete random variable $Y$ and a density function $U = h(Y)$ ($U$ and $Y$ should be one to one corresponding). We want to find the probability density function $f_U(U)$.

1. we need to first find the inverse function of $h(Y)$: $h^{-1}(u)$.
2. After that, we can use the formula 

    $$
    f_U(u) = f_Y(h^{-1}(u))
    $$

## function of discrete random variables

We are given a probability density function $f(Y_1,Y_2)$ of  discrete random variables $Y_1$ and $Y_2$ and  a density function $X_1 = h_1(Y_1,Y_2)$ and $X_2 = h_2(Y_1,Y_2)$. We want to find the probability density function $g(X_1,X_2)$. We can use the method below:

1. find $Y_1 = w_1(X_1,X_2)$ and $Y_2=w_2(X_1,X_2)$

2. $g(X_1,X_2) = f(w_1(X_1,X_2),w_2(X_1,X_2))$

# continuous type 

We are given a probability density function $f_Y(Y)$ of a continuous random variable $Y$ and a density function $U = h(Y)$ which must have inverse function[^2](one to one corresponding). we want to find the probability density function $f_U(U)$.

1. we need to first find the inverse function of $h(Y)$: $h^{-1}(u)$.
2. After that, we can use the formula 

    $$
    f_U(u) = f_Y(h^{-1}(u))|\frac{dh^{-1}}{du}|
    $$

## why this method works?

It is because that for $h(Y)$ being an increasing or decreasing function, every $y$ can be uniquely mapped to a $u$ where $F_U(u) = F_Y(y)$, thus [[differentiate]] both side will give us the formula above. 

## functions of continuous random variables

We are given a probability density function $f(Y_1,Y_2)$ of  continuous random variables $Y_1$ and $Y_2$ and  a density function $X_1 = h_1(Y_1,Y_2)$ and $X_2 = h_2(Y_1,Y_2)$. We want to find the probability density function $g(X_1,X_2)$. We can use the method below:

1. find $Y_1 = w_1(X_1,X_2)$ and $Y_2=w_2(X_1,X_2)$

2. $g(X_1,X_2) = f(w_1(X_1,X_2),w_2(X_1,X_2))|J|$    Where $J$ is the determinant of [[Jacobian matrix]]. 
‍

# If not one to one corresponding

We can divide the function into different parts which in this part random variables are one to one corresponding and calculate the density functions and add them. 

‍
1. [(583) MA 381: Section 6.2: Functions of a Random Variable Example Worked Out at a Whiteboard - YouTube](https://www.youtube.com/watch?v=H00rv6jVwrI)