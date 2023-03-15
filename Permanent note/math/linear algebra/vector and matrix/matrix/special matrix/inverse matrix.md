#linear_algebra 
For a matrix A, if it has $CA = I = AC$
we call $C =A^{-1}$ as the inverse matrix of $A$

# when inverse matrix exists? 
Matrix $A$ is [[invertible]] $\iff$ $det (A) \neq 0$ ( $det (A)$ is the [[determinant]] of $A$ ) 

# Properties
1. $(ABC)^{-1} =C^{-1}B^{-1}A^{-1}$

## calculation of inverse matrix
1.  $\begin {bmatrix} A & I \end{bmatrix}$  to  $\begin {bmatrix} I & A^{-1} \end{bmatrix}$ using [[gaussian elimination]] 
2. $(A^{-1})_{ij} = \frac{1}{C_ij}{det (A)}$ and  $A^{-1} = (\frac{1}{detA})C^T$
$C$ is the [[cofactor matrix]] and $C_{mn}$ is the [[cofactor]] of $A_{mn}$  
([“introduction to linear algebra”, p. 285](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=285&annotation=HSWI5DKS))  

