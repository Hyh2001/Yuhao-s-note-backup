#robotics/robot_motion
* [ ] The definition of exponential coordinate maybe wrong? 

Exponential coordinate can be used to represent transformations or rotations of a robot. If given a [[screw axis]] $S = (\omega,v)$, then we can define the exponential coordinate as $e^{[S]\theta}=\begin{bmatrix} e^{[\omega]\theta} & (I\theta + (1-cos\theta)[\omega] + (\theta-sin\theta)[\omega]^2)v \\ 0 & 1 \end{bmatrix}$ if $||\omega|| = 1$  

or, 

$e^{[S]\theta}=\begin{bmatrix} I & \theta v \\ 0 & 1 \end{bmatrix}$ if $||\omega|| = 0$ and $|| v|| = 1$ 

## exponential coordinate representation of rotation

Exponential coordinate is used to represent [[rotation]]s of a robot. We can represent a [[matrix logarithm]] in terms of a rotation axis by a unit vector $\vec{\omega}$ and an angle or rotation about that vector $\theta$. Then the exponential coordinate is defined as $\vec{\omega}\theta$.why this representation works? 

#todo

## what is its advantages?

1. It does not suffer from [[singularity]]. 
2. screw theory always gives an entirely geometric description of the rigid body motion, which significantly simplifies the analysis of mechanisms in robotics.

# programming implementation

```matlab
% extract rotation axis and rotation amount from exponential coordinates 
[omega,theta] = AxisAng3(expc3)
```

1. [Lynch_Park_2017_Modern robotics - Excerpt of: Lynch_Park_2017_Modern robotics, p97](lt://open/sF1mSW5VQE-dMECpL20GNA)
2. Advantages of using exponential coordinate ([Pardos-Gotor, 2021, p. 24](zotero://select/library/items/V6J2RZZH)) ([pdf](zotero://open-pdf/library/items/9ZMQK9KL?page=51&annotation=A5K4V6XU))