---
aliases: [homogeneous transformation matrix]
sr-due: 2023-01-15
sr-interval: 3
sr-ease: 250
---
#robotics/robot_motion  #review 
Special Euclidean group also known as group of rigid-body motions or [[homogeneous transformation matrix]] is denoted as $SE(3)$. It is a [[group]] . It is a $4 \times 4$ matrix in the form

$T = \begin{bmatrix} R & p \\ 0 & 1     \end{bmatrix} = \begin{bmatrix} r_11 & r_12 & r_13 & p_1 \\ r_21 & r_22 & r_23& p_2\\ r_31 &r_32 &r_33 & p_3 \\ 0& 0&0&1 \end{bmatrix}$ where $R \in SO(3)$ is a [[rotation matrix]] and $p \in \mathbb{R}^3$ a column vector. 

This matrix is used to transform [[homogeneous coordinate]]s. 

## for planar transformation

For planar transformations, the special Euclidean group is defined as $SE(2)$ which is a $3 \times  3$ matrix has the form: 

$T = \begin{bmatrix} R & p \\0 & 1     \end{bmatrix}$ where $R \in SO(2)$ and $p \in \mathbb{R}^2$ 

# properties of special Euclidean group

## follows the properties of groups：

1. $T^{-1} = \begin{bmatrix} R^T & -R^Tp \\ 0 & 1     \end{bmatrix}$ is also a transformation matrix
2. product of two transformation matrix is also a transformation matrix
3. The multiplication of transformation matrices is associative but not commutative

## preserves distances and angles

1. $||Tx -Ty|| = || x-y||$ where $|| \cdot ||$ denotes the [[standard Euclidean norm]] in $\mathbb{R}^3$ and $x,y \in \mathbb{R}^3$
    ‍
2. $<Tx -Tz, Ty- Tz> = <x-z,y-z>$ for all $z,x,y \in \mathbb{R}^3$,where $< \cdot,\cdot>$ denotes the [[standard Euclidean inner product]] in $\mathbb{R}^3$

‍

# application of special Euclidean group

## representing a configuration 

$T_{bc}$ represents $\{b\}$ relative to $\{c\}$ 

## changing the reference frame of a vector or a frame

$T_{ab}T_{bc} = T_{ac}$ and $T_{ab}v_b = v_a$

## transforming a vector or a frame

### versus reference frame

$T_{sb^{'}} = TT_{sb} = \begin{bmatrix} RR_{sb} & Rp_{sb} + p \\ 0 &  1\end{bmatrix}$

### versus body frame

$T_{sb^{''}} = T_{sb}T = \begin{bmatrix} R_{sb}R & R_{sb}p + p_{sb} \\ 0 &  1\end{bmatrix}$  


# [[adjoint representation of special Euclidean group]]
# exponential coordinate representation 
see [[exponential coordinate]], $T = e^{[S]\theta}$

# programming implementation

```matlab
% compute the inverse of a homogeneous transformation matrix
invT = TransInv(T)
% compute homogeneous transformation matrix from rotation matrix and position vector
T = RpToTrans(R,p)
% find the adjoint representation of homogeneous transformation matrix
AdT = Adjoint(T) 
% find transformation matrix from matrix exponential
T = MatrixExp6(se3mat)
```
