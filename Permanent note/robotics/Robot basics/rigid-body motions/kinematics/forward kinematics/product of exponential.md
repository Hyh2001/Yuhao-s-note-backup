The product of exponential method is a method that implements the [[screw theory]]. Its steps are listed below: 
1. Select the [[reference frame]] $S$ (usually at robot’s base) and the [[body frame]] $T$ of the [[end-effector]]. 
2. Define the axis of each [[joint]] with respect to the reference frame( [[rotation axis]]  $\omega$ for [[revolute joint]], sliding direction $v$ for [[prismatic joint]] s, a point $q$ on those axes) 
3. Calculate the [[twist]] for the joints. 
4. Find the reference [[pose]] of the end-effector  $H_{ST}(O)$ 
5. solve the equation below which is the POE formula to find joint magnitudes. 
$$
H_{ST}(\theta) = \prod_{i=1}^{n}e^{[V_i]\theta_i}H_{ST}(0)
$$
 ([Pardos-Gotor, 2021, p. 37](zotero://select/library/items/V6J2RZZH)) ([pdf](zotero://open-pdf/library/items/9ZMQK9KL?page=64&annotation=H8PNXM8Y))


[[body form of product of exponential]]