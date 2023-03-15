#robotics/robot_motion #linear_algebra 
 
Given a [[angular velocity]] vector $x = [x_1 \quad x_2 \quad  x_3]^T \in \mathbb{R}^3$ 

we can define::

$[x] = \begin{bmatrix}0 & -x_3 & x_2 \\ x_3 & 0 & -x_1 \\ -x_2 & x_1 & 0 \end{bmatrix}$ This is the skew-symmetric matrix of $x$
([Lynch 和 Park, 2017, p. 95](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=95&annotation=G8B9YTYP))

This matrix is used to represent a **[[cross product]]** which $\omega \times x = [\omega]x$  
# property

It has the property that:: $[x] = -[x]^T$. The set of all 3 by 3 real skew-symmetric matrices is called :: $so(3)$ ([[Lie algebra]]).

# programming implementation

```matlab
% find the skew-symmetric form of a vector omg
so3mat = VecToso3(omg)
% find the  3 by 3 vector correspond to a skew-symmetric matrix
omg = so3ToVec(so3mat)
```
# skew-symmetric matrix representation of a [[spatial velocity]] 
Let $x$ denotes a spatial velocity $x = [w_1,w_2,w_3,v_1,v_2,v_3]$, its skew-symmetric matrix is defined as::
$[x] = \begin{bmatrix} [w] & v \\ 0 & 0 \end{bmatrix}$  
 


    ‍
