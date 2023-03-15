#robotics/robot_motion 

For matrix logarithm, we can consider a transformation matrix $T$ or a rotation  matrix $R$, use [[Rodrigues formula]] we can prove that $T = e^{[\vec{S}]\theta}$ or $R = e^{[\vec{\omega}]\theta}$. And we denote that $[\vec{S}]\theta$ as the matrix logarithm of $T$ and $[\vec{\omega}]\theta$ as the matrix logarithm of $R$ (rotation matrix).
# matrix logarithm of [[homogeneous transformation matrix]]
We can find that $[S]\theta = \begin{bmatrix} [\omega]\theta & v\theta \\ 0 & 0 \end{bmatrix}$  

1. If $R =I$ then, $\omega = 0$, $v= p/||p||$ and $\theta = ||p||$
2. Otherwise, we can first use matrix logarithm of $SO(3)$ provided below to determine $\omega$ and $\theta$ for $R$ and then $v= G^{-1}(\theta)p$ where $G^{-1}(\theta) = \frac{1}{\theta}I - \frac{1}{2}[\omega] + (\frac{1}{\theta} - \frac{1}{2}cot\frac{\theta}{2})[\omega]^2$

# matrix logarithm of [[rotation matrix]]

If we are given a $R \in SO(3)$, and we are required to find a $\theta$ and a $\vec{\omega}$ versus $R$, so that $[\vec{\omega}\theta] \in so(3)$ is the matrix logarithm of $R$ 

They are denoted as below:

1. If $R = I$, then $\theta = 0$ and $\vec{\omega}$ is undefined
2. If $tr R= -1$( "$trR$" is the [[trace]] of $R$) then $\theta = \pi$ and 

    $$
    \omega = \frac{1}{\sqrt{2(1+r_{11})}}\begin{bmatrix} 1+r_{11} \\ r_{21} \\ r_{31} \end{bmatrix} = \frac{1}{\sqrt{2(1+r_{22})}}\begin{bmatrix} r_{12} \\ 1+ r_{22} \\ r_{32} \end{bmatrix}  = \frac{1}{\sqrt{2(1+r_{33})}}\begin{bmatrix} r_{13}\\ r_{23} \\1+ r_{33} \end{bmatrix}
    $$

3. otherwise, $\theta = cos^{-1}(\frac{1}{2}(trR-1)) \in [0, \pi)$ and $[\vec{\omega}] = \frac{1}{2sin\theta}(R-R^T)$

## proof
#todo 
‍

# programming implementation

```matlab
% compute matrix logarithm of rotation matrix
so3mat = MatrixLog3(R)
% compute matrix logarithm of transformation matrix
se3mat = MatrixLog6(T) 
```

‍

‍

‍

1. [robotics - Excerpt of: Lynch_Park_2017_Modern robotics, p124](lt://open/gS_Jo0SwKEmHvfoSN5o6Hw)
2. [Project - Lynch_Park_201...](lt://open/okilcpCd0Uat-3g80r-yAg)

‍
