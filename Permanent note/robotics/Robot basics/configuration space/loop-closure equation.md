They are a group of equations that can implicitly define a closed-chain mechanism.

# for a four bar linkage

![[Pasted image 20221027164310.png]]
We can three equations:

1. $L_1cos\theta_1 + L_2cos(\theta_1 + \theta_2) + ... + L_4cos(\theta_1 + \theta_2 + \theta_3 + \theta_4) = 0$
2. $L_1sin\theta_1 + L_2sin(\theta_1 + \theta_2) + ... + L_4sin(\theta_1 + \theta_2 + \theta_3 + \theta_4) = 0$
3. $\theta_1 + \theta_2 + \theta_3 + \theta_4 - 2\pi = 0$
   The solution of these equations form a one-dimensional curve in the four-dimensional space

# for general cases

We can implicitly use column vectors $\theta = [\theta_1 , \theta_2 , \theta_3 , \theta_4]^T$ to implicitly represent the configuration space. (***Because of constraints, the dof must less than $nn$) We will have the loop-closure equation as the form.  
$g(\theta) = \begin{bmatrix} g_1(\theta_1,...\theta_n) \\ . \\. \\. \\ g_k(\theta_1,...,\theta_n)\end{bmatrix} = 0$, $k \leq n$  
The equations are constraints and thus $k$ is the number of constraints. These constraints are called [[holonomic constraint]]s or [[integrable constraint]]s. The configuration space can be viewed as a surface of dimension $n-k$ embedded in $\mathbb{R}^n$.  
We differentiate $\theta$ with respect to $t$, we will have $\frac{d}{dt}g(\theta(t)) = 0$  
by using [[chain rule]]:  
$\begin{bmatrix} \frac{\partial g_1}{\partial \theta_1}(\theta)(\dot{\theta_1}) + ... + \frac{\partial g_1}{\partial \theta_n}(\theta)(\dot{\theta_n})\\ . \\. \\. \\ \frac{\partial g_k}{\partial \theta_1}(\theta)(\dot{\theta_1}) + ... + \frac{\partial g_k}{\partial \theta_n}(\theta)(\dot{\theta_n})\end{bmatrix} = 0$  
let $\dot{\theta_n}$ out$\begin{bmatrix} \frac{\partial g_1}{\partial \theta_1}(\theta) + ... + \frac{\partial g_1}{\partial \theta_n}(\theta)\\ . \\. \\. \\ \frac{\partial g_k}{\partial \theta_1}(\theta) + ... + \frac{\partial g_k}{\partial \theta_n}(\theta) \end{bmatrix} \begin{bmatrix}\dot{\theta_1} \\. \\. \\. \\ \dot{\theta_n} \end{bmatrix} = 0$ in short, it is $\frac{\partial g}{\partial \theta}(\theta)\dot{\theta} = 0$, let $A(\theta) = \frac{\partial g}{\partial \theta}(\theta)$, we can have $A(\theta)\dot{\theta} = 0$, $A(\theta)$ which is the velocity constraint is also called Pfaffian constraint.  
Sometimes, for some Pfaffian constraints, they are not [[Integrable]] which means that $g(\theta)$ does not exist. These constraints are called [[nonholonomic constraint]]. (They usually occur in rolling without slipping and conservation of momentum)
