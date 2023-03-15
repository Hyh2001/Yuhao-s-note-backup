---
sr-due: 2023-02-19
sr-interval: 3
sr-ease: 250
---

#linear_algebra #review 

Determinant is a [[function]] that maps a [[square matrix]] to a real number and it is noted as $det A$ or $|A|$. It can be used to determine whether a square system of linear equations have a unique solution. ($detA = 0$ means there is no solution )

# properties

For determinant, it has three basic properties with more 8 properties can be got from the three basic ones.  To compute the determinant, we need to first understand [[cofactor]] s. With cofactors we can compute the [[inverse matrix]]  of a square matrix and moreover use [[Cramer's rule]] to compute x.

1. $det I = 1$ where $I$ is the [[identity matrix]] ([“introduction to linear algebra”, p. 259](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=259&annotation=9T4A8NUJ))

2. If you exchange two rows of a determinant, it reverses the sign of the determinant. $\begin{vmatrix}c &d \\ a &b \end{vmatrix} = -\begin{vmatrix} a &b \\c &d \end{vmatrix}$ ([“introduction to linear algebra”, p. 259](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=259&annotation=RMYPTAD2))
3. multiply one row by $t$, $\begin{bmatrix} ta & tb\\ c& d \end{bmatrix} = t\begin{bmatrix} a & b\\ c& d \end{bmatrix}$, add between rows $\begin{vmatrix} a+e & b+f\\ c& d \end{vmatrix} = \begin{vmatrix} a & b\\ c& d \end{vmatrix} + \begin{vmatrix} e &f\\ c& d \end{vmatrix}$, $det (zA) = z^ndet(A)$ $z$ is a number ([“introduction to linear algebra”, p. 259](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=259&annotation=X4EAS5XW))

4. If two rows are equal, $det(A) = 0$  
    Prove: two rows are equal, then change these two rows will get the formula $det (A) = -det(A)$ which mans that $det (A) = 0$ ([“introduction to linear algebra”, p. 260](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=260&annotation=2FMJZTXT))
5. subtract $l*row 1$ from $row k$ ,the determinant will not change  
    Prove: $\begin{vmatrix} a & b\\ c-la& d-lb \end{vmatrix} = \begin{vmatrix} a & b\\ c& d \end{vmatrix} + \begin{vmatrix} a &b\\ -la& -lb \end{vmatrix} = \begin{vmatrix} a & b\\ c& d \end{vmatrix} + 0$
	([“introduction to linear algebra”, p. 260](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=260&annotation=4NKCDP3N))
6. Row of zeros will lead to $det A = 0$
	Prove: You can simply construct two equal rows in this situation 
	 ([“introduction to linear algebra”, p. 260](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=260&annotation=XFDD8DAV))
7. For a triangular matrix , $det A$ equals to the product of its diagonals
	Prove: We can construct a [[diagonal matrix]] by simply using [[gaussian elimination]] without changing the determinant. Then by using rule 3 to factor all of the [[diagonal]] s out and we can prove the property. If there produces a 0 on diagonal then $det (A) = 0$ ([“introduction to linear algebra”, p. 261](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=261&annotation=6NKFHKJ3))
	
8. $det A =0$ When $A$ is a [[singular matrix]] 
	Prove: If $A$ is singular then by elimination there is a zero row inside $A$  ([“introduction to linear algebra”, p. 261](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=261&annotation=6C6RDSJ6))

9. $det AB = (det A) (det B)$ And $det A^{-1} = 1/ det A$ ,  
	Prove: $det (I) =det (AA^{-1}) = 1$  ([“introduction to linear algebra”, p. 262](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=262&annotation=CVJ8A8KC))

10. $det A^T = det A$  
     Prove: By using [[LU factorization]], $|A^T| = |A| => |U^TL^T| = |LU| => |U^T||L^T| = |L||U|$ ([“introduction to linear algebra”, p. 262](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=262&annotation=DMJPNYTZ))

# three methods to calculate determinants 
## pivot formula 
$det (A)$ equals to the product of [[pivot]] s  of $A$ ([“introduction to linear algebra”, p. 268](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=268&annotation=WLNJKVKA))

proof: We know that $det (A) =det(L)det(U)$ by [[LU factorization]], $det (L) = 1$ for all the diagonal entries are 1, and $det(A) = det(U)$ where diagonal entries of $U$ are pivots of $A$  ([“introduction to linear algebra”, p. 268](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=268&annotation=P2QDV49D))
## big formula 
$det (A) =$ sum over all $n!$ column permutations $P = (\alpha,\beta,\ldots,\omega)$ = $\sum (detP) a_{1\alpha}a_{2\beta}\ldots a_{n\omega}$  ([“introduction to linear algebra”, p. 271](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=271&annotation=W5VZH47M))  
## [[cofactor]] formula 
for cofactor $C_{ij} = (-1)^{i+j}detM_{ij}$
The determinant is $detA = a_{1j}C_{1j} +a _{2j}C_{2j}+…+a_{nj}C_{nj}$
([“introduction to linear algebra”, p. 274](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=274&annotation=KJXVGT9X))  
advantages of this calculation method: 
1. It is useful when matrices have many zeros. ([“introduction to linear algebra”, p. 274](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=274&annotation=M92K8WD8)) 

# applications of determinants 
## 1.  [[Cramer’s rule]] 

## 2. Find [[inverse matrix]] 


## 3. use determinant to find areas and volumes
### volume of a triangle 
If we know the three corners of a triangle $m$ and one of its corner $(x_3=0,y_{3}=0)$, then we can calculate its area as: 
$Area = \frac{1}{2}|det(\begin{bmatrix} x_{1}&y_{1}&1 \\ x_2&y_{2}&1\\ x_{3}&y_{3}&1\end{bmatrix})|$ 
([“introduction to linear algebra”, p. 286](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=286&annotation=R5HBPIGN))  

### volume of n-dimensional geometries 
The volume equals $|det(A)|$ ([“introduction to linear algebra”, p. 288](zotero://select/library/items/4K5E75TP)) ([pdf](zotero://open-pdf/library/items/LM7HCCN7?page=288&annotation=8RPKV7CK))

### sign of determinants:
Tell us whether the box is [[right-handed]] or left-handed 
## 4. [[cross product - determinant]]
[[triple product]] 
# programming implementation 
```julia
using Pkg
Pkg.add("LinearAlgebra")
using LineraAlgebra

A = [1 1 ;2 2]
det(A) #A is a square matrix
```

