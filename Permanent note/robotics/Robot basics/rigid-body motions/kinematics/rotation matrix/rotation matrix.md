#robotics/robot_motion 

Rotation matrix is a 3 by 3 matrix whose purpose is to perform [[rotation]]s of vectors in [[Euclidean space]]. All of the rotation matrices form a set called [[special orthogonal group]].
# why a rotation matrix can represent a rotation 
Let us define a rotation for a [[reference frame]] $A$ to a [[body frame]] $B$. We can easily write the coordinates of three axes of $B$ with respect to $A$ as $[_Ae^B_x,_Ae^B_y,_Ae^B_z]$. 
Therefore,  for a point $P$ in the coordinate systems $P_{A}= [_Ae^B_x,_Ae^B_y,_Ae^B_{z}] \cdot P_{B}$ and we define $[_Ae^B_x,_Ae^B_y,_Ae^B_{z}]$ as the rotation matrix. 
([“robot dynamics lecture note”, p. 9](zotero://select/library/items/TGHFK5DD)) ([pdf](zotero://open-pdf/library/items/XC5MH7YR?page=14&annotation=X8FLYWFE))

# properties of rotation matrix

## constraints 

For rotations in a three-dimensional space, 3 [[degree of freedom]]s are permitted which means that only 3 of 9 numbers can be randomly chosen in the matrix. Therefore, 6 constraints should be applied. There are two types: 

### Unit norm condition

Three columns of the matrix should be unit vectors 

$\begin{matrix}r_{11}^2 + r_{21}^2+r_{31}^2 =1 \\  r_{12}^2 + r_{22}^2+r_{32}^2 =1 \\ r_{13}^2 + r_{23}^2+r_{33}^2 =1  \end{matrix}$

### orthogonality condition

Three columns should be orthogonal. 

$\begin{matrix}r_{11}r_{12} + r_{21}r_{22}+r_{31}r_{22} =0 \\  r_{12}r_{13} + r_{22}r_{23}+r_{32}r_{33} =0 \\ r_{13}r_{11} + r_{23}r_{21}+r_{33}r_{31} =0  \end{matrix}$ 

And finally, group all the constraints together, we can have: (they are only valid [[right-handed]] systems. For left-handed, the [[determinant]] will be -1.

$$
R^TR = I \quad or \quad det R =1
$$


# applications of rotation matrix
## represent orientation of a reference frame

$R_{sc}$ means that for a frame $c$, its orientation versus frame $s$ is $R_{sc}$

## change the reference frame of a vector or a frame

$R_{ac} = R_{ab}R_{bc}$, this equation will change frame or vector $c$ from versus $b$ to versus $a$

## rotate a vector or a frame
### versus reference frame 

$v^{'} = R_{ss}v$ where $R_{ss}$ (This means that the frame in which we represent the angular velocity is the reference frame. and $v$ should be **represented in the same frame. )**

### versus body frame 

$v^{''} = vR_{bb}$ where $R_{bb}$ (This means that the frame in which we represent the angular velocity is the body frame. and $v$ should be **represented in the same frame. )**

# rate of change of rotation matrix

For a constantly moving body, its representation of orientation versus the [[reference frame]] which is denoted by $R$ is constantly changing. We use $\dot{R}$ to denote rate of changing of this frame. Then, for a pure rotation: 
$\dot{R_{s}} = \omega_s \times R_{s}$ where $\omega_s$ is the [[angular velocity]] versus the fixed frame. ([Lynch 和 Park, 2017, p. 94](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=94&annotation=HJ9GS4LV))
![[Pasted image 20230212083127.png]]

## introduction of [[skew-symmetric matrix]]
We then rewrite the angular velocity into its skew-symmetric matrix form and we can see that :: $\dot{R} = [\omega_s]R \to  [\omega_s] = \dot{R}R^{-1}$ . 

with the [[rotation matrix proposition 3.8]] we can proof that :: $[\omega_b] = R^{-1}\dot{R}$
([Lynch 和 Park, 2017, p. 97](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=97&annotation=4B9NVXKD))  

Their relationship can be simply built by $\omega_{b}=R_sb\omega_{s}$ ([Lynch 和 Park, 2017, p. 97](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=97&annotation=N3HNULYX))
# [[rotation matrix - rotation axis - angular coordinate]]
# [[exponential coordinate]] representation of rotation matrix

# programming implementation

```matlab
% find the inverse of a rotation matrix
invR = RotInv(R) 
% computer rotation matrix from matrix exponential
R = MatrixExp3(R)
% extract rotation matrix and position vector from transformation matrix
[R,p] = TransToRp(T)
```

‍

‍

‍

‍

1. [Lynch_Park_2017_Modern robotics - Excerpt of: Lynch_Park_2017_Modern robotics, p82](lt://open/dHkbI9lPGUas8yqPTuTpEA)

2. [Murray et al_1994_A mathematical introduction to robotic manipulation - Excerpt of: Murray et al_1994_A mathematical introduction to robotic manipulation, p44](lt://open/3IqAUphAkEOUtHQhsIB0EQ)
