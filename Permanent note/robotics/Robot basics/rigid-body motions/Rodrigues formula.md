#robotics/robot_motion #todo 
This formula states that: given a vector $\vec{w}\theta \in \mathbb{R}^3$, such that $\theta$ is any scalar and $\vec{\omega} \in \mathbb{R}^3$ is a unit vector which denotes the rotation axis, the [[matrix exponential]] of $[\vec{\omega}]\theta = [\vec{\omega}\theta] \in so(3)$ is ::
$Rot(\vec{\omega},\theta) = e^{[\vec{\omega}]\theta} = I + sin\theta[\vec{\omega}] + (1-cos\theta)[\vec{\omega}]^2 \in SO(3)$ and finally:

$e^{[\vec{\omega}]\theta} =$ ![[Pasted image 20221222102845.png]]
$s\theta =sin \theta$ and $c\theta = cos\theta$ 

$[  \quad ]$ operator is to find the [[skew-symmetric matrix]] form of a vector.

# proof 

For rotating a vector $p$ with [[angular velocity]] $\vec{\omega}$, we can have the formula represents the **linear velocity** of point $p$ as ::
$\dot{p} = \vec{\omega} \times p$ 

It can be then denoted as:

$\dot{p} = [\vec{\omega}]p$  and we find that it is a differential equation which has the form of a [[linear system]] whose solution is denoted as $p(t) = e^{[\vec{\omega}]t} p_0$. We can use $\theta$ to replace $t$ for they are interchangeable(​*why they are interchangeable?*).

now we expand $e^{[\vec{\omega}]\theta}$ with the property of skew-symmetric matrix that $[\vec{\omega}]^3 = -[\vec{\omega}]$. We then get the formula.

‍