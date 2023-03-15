# projection

# math model

## For two-dimensional:

if we vector $b$ onto a subspace with its basis be $a$ (the subspace can be represented as $p = ca$ )
we will have:
1.$a^T(b- ca) = 0$, $c$ is scalar
2.we can have c = $a^Tb/a^Ta$
3.$P =a (a^Tb/a^Ta)$

## For n-dimensional:

using a matrix $P = A(A^TA)^{-1}A^T$ to represent projection

### properties:

1.symmetric matrix[^1]  
2.$P^2 = P$  
3.$pb = b$ for $b$ is in the column space  
4.$pb = 0$ for $b$ is orthogonal to the column space<br />5.the projection matrix corresponding to $e$ is $P_e = (I-p)b$  

# why we need projection:

1.to solve $Ax = b$ by using $A\hat{x} = p$ which p is the projection of $b$ on column space of $A$  
2.$error =b - p = b - A\hat{x}$ and we can see that $error$ is perpendicular to the column space of $A$ which is in the left nullspace[^2]  
3.$A^T(b-A\hat{x}) = 0$  
​$\hat{x}= (A^TA)^{-1}A^Tb$  
​$p = A\hat{x} = A(A^TA)^{-1}A^Tb$  
4.projection matrix:  
​$P = A(A^TA)^{-1}A^T$  

‍

[^1]: # symmetric matrix

    If a matrix A is symmetric, then $A^T = A$  

    ## applications

    1. $A^TA$ is a symmetric matrix:  
       proof:  $(A^TA)^T = A^T(A^T)^T  = A^TA$  
       So, if A is symmetric, then its $LDU$ decomposition becomes  
       $A = LDU = LDL^T$


[^2]: # left nullspace

    # definition

    The null space of $A^Ty = 0$

    ## properties
