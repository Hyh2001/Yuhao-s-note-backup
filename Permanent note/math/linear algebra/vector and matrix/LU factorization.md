LU factorization is a method that we can factorize an arbitrary [[matrix]] into an [[upper-triangular matrix]] and a [[lower-triangular matrix]] which we denote them $U$ and $L$.  
We use  $A = PLU$, where $P$  is the [[permutation matrix]] to denote the factorization. 

# method to find L and U 
For a [[square matrix]] $A$ we can use $\begin{bmatrix} a_{11} & a_{12} & \ldots & a_{1n} \\ a_{21} & a_{22} & \ldots & a_{2n} \\ \ldots & \ldots & \ldots & \ldots \\ a_{n1} & a_{n2} & \ldots & a_{nn}  \end{bmatrix}$ to denote it. 
We can find that actually: $A - \begin{bmatrix} \frac{a_{11}}{a_{11}} \\ \frac{a_{21}}{a_{11}} \\ \ldots \\ \frac{a_{n1}}{a_{11}}  \end{bmatrix} \cdot \begin{bmatrix} a_{11} & a_{12} & \ldots & a_{1n} \end{bmatrix} = \begin{bmatrix}0 & 0 & \ldots & 0 \\ 0 & * & \ldots & * \\ \ldots & \ldots & \ldots & \ldots \\ 0 & * & \ldots & * \end{bmatrix}$ where $*$ are arbitrary numbers. 
Therefore, by iteratively performing these steps we can finally finish LU factorization. 
## why we need permutation matrix? 
Some matrices will not have LU factorization without row permutations. There are several situations: 
1. There are $0$ on [[pivot]] s. 
## special cases 
### entire columns of zeros 
$A = \begin{bmatrix} 0 & 0& 0 \\ 0 & 0 & 3 \\ 0 & 0 & 4 \end{bmatrix}$ 
we can define $C = \begin{bmatrix} 0 \\1\\0 \end{bmatrix}$ and $R = \begin{bmatrix} 0 & 0& 3 \end{bmatrix}$ 
In general, at the $k$ -th step, if C becomes a column of all zeros, set its $k$ -th entry to one and define R as usual
### pivot value is zero 
perform row permutations. 
# applications 

use [[back substitution]] to solve systems of [[linear equation]] s .
We can have $A = PLU$ and $PLUx = b$
$Ux = L^{-1}P^{-1}b$

# julia implementation
## without permutations 
```julia 
Temp = copy(A)
nRows, nCols = size(Temp)
L = Array{Float64,2}(undef,nCols,0)
U = Array{Float64,2}(undef,0,nRows)
for k = 1:nRows 
	@show Temp 
	pivot = Temp[k,k]
	if ! isapprox(pivot,o,atol = 1E-8)
		C = Temp[:,k]/pivot 
		R = Temp[k:k,:]
		Temp = Temp - C*R
		L = [L C]
		U = [U;R] 
	else 
		println("Matrix requires row permutations to avoid zero")
		println("Step where algorith failed is k =$k")
		break
	end 
@show Temp
return L,U
```
## with permutations 
```julia 
Temp = copy(A)
nRows, nCols = size(Temp)
L = Array{Float64,2}(undef,nCols,0)
U = Array{Float64,2}(undef,0,nRows)
P = zeros(nRows,nCols) + I
eps = 1e-16 
kappa = 10 
for k=1:n 
	C=Temp[:,k]; # k-th column 
	if max(abs(C)) <= Kappa*eps # (check for C all zeros) 
	C=0*C # Set tiny values to zero 
	C[k]=1.0 
	R=Temp[k:k,:] # k-th row 
	Temp=Temp-C*R L=[L,C] # Build the lower-triangular matrix by columns 
	U=[U;R] # Build the upper-triangular matrix by rows 
	else 
	# We know C has at least one non-zero quantity 
	# We’ll bring its largest entry to the top; 
	# while this is overkill, it helps with numerical aspects of the algorithm 
	# Bringing biggest to top will always avoid divide by zero 
	# It’s enough to bring ANY non-zero value to the top 
	# 
	nrow=argmax(abs(C)) # find the index where C is “biggest” 
	P[[k,nrow],:]=P[[nrow,k],:] # permute (i.e., swap) rows of P
	Temp[[k,nrow],:]=Temp[[nrow,k],:] # do same for Temp 
	# if L is non-empty, also swap its rows 
	if k > 1 L[[k,nrow],:]=L[[nrow,k],:] end 
	C=Temp[:,k]; # k-th column 
	pivot = C[k] C=C/pivot #divide all elements of C by the pivot 
	R=Temp[k:k,:] # k-th row 
	Temp=Temp-C*R 
	L=[L C] # Build the lower-triangular matrix by columns 
	U=[U;R] # Build the upper-triangular matrix by rows 
	end 
end 
return L, U, P
```
## julia APIs  ```

```julia
using LinearAlgebra 
# with no permutations 
L, U = lu(M,Val(false)) # Val(false) means that we don't apply row permutations 
# with permutations 
F = lu(M) 
L =F.L 
U =F.U
P =F.P
```


1. factorization method ([Grizzle, p. 69](zotero://select/library/items/8EBIR37H)) ([pdf](zotero://open-pdf/library/items/2AVWIQEV?page=69&annotation=7WJ6BX89))
2. julia code without permutations ([Grizzle, p. 71](zotero://select/library/items/8EBIR37H)) ([pdf](zotero://open-pdf/library/items/2AVWIQEV?page=71&annotation=YI4C37JL))
3. julia code with permutations ([Grizzle, p. 84](zotero://select/library/items/8EBIR37H)) ([pdf](zotero://open-pdf/library/items/2AVWIQEV?page=84&annotation=K99ASSIZ))
4. jula APIs ([Grizzle, p. 72](zotero://select/library/items/8EBIR37H)) ([pdf](zotero://open-pdf/library/items/2AVWIQEV?page=72&annotation=TIGWC9KQ))
5. why we need permutation matrix  ([Grizzle, p. 78](zotero://select/library/items/8EBIR37H)) ([pdf](zotero://open-pdf/library/items/2AVWIQEV?page=78&annotation=J87MTG34))
6. special case 1  [Grizzle, p. 81](zotero://select/library/items/8EBIR37H)) ([pdf](zotero://open-pdf/library/items/2AVWIQEV?page=81&annotation=P5XT442M))