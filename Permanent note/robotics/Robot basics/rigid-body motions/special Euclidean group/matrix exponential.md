#linear_algebra #robotics/robot_motion

Matrix exponential is defined as follow: 

$e^{At} = I + At + \frac{(At)^2}{2!} + \frac{(At)^3}{3!} + ...$  

## proof
#todo
# convergence
If $A$ is constant and finite then this series is always guaranteed to converge to a finite limit. 
## proof
#todo
* [ ] why we are interested in the convergence of matrix exponential?


# properties of matrix exponential 
For $e^{At}$, we can see that they satisfy some properties: 
1. $\frac{d(e^{At})}{dt} = Ae^{At} = e^{At}A$
2. If $A = PDP^{-1}$ for some $D \in \mathbb{R}^{n \times n}$ and invertible $P \in \mathbb{R}^{n \times n}$ then, $e^{At} = Pe^{Dt}P^{-1}$
3. If $AB =BA$ then $e^Ae^B =e^ {A+B}$
4. $(e^A)^{-1} = e^{-A}$

 
‍

‍

‍

‍

‍

‍

1. [Project - Lynch_Park_201...](lt://open/bfxPmQf6qUmNwePRmDiEhQ)

‍
