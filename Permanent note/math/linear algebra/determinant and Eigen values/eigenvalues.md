#linear_algebra 

For $Ax = \lambda x$ , $\lambda$ is a multiple of $x$ and is called an eigenvalue

## properties
1.If $\lambda = 0$, then $x$ is the [[nullspace]]  of $A$  
2.sum of eigenvalues equal to the trace of $A$  
3.for symmetric matrix, eigenvalues are real numbers  
4.for anti-symmetric matrix, eigenvalues are pure imaginary numbers  
5. add $nI$ to $A$ will cause eigenvalues become $(\lambda+n)x$. product of eigenvalues equal to the determinant  
7.for a triangular matrix, their eigenvalues are on their diagonals  
8.eigenvalues of $A^2$ are $\lambda ^2$  
9.tell us the growth rate of a dynamic problem

## find of eigenvalues and eigenvectors

### for a projection matrix

Eigenvectors are the vectors that

#### 1.in the plane

And eigenvalues are 1

#### 2.are perpendicular to the plane

And eigenvalues are 0

### for all matrix

$(A-\lambda I)x = 0$
And $A-\lambda I$ must be singular for $x$ is not only zero vectors

#### characteristic equation

$det(A-\lambda I) = 0$

#### solve for $\lambda$

$\lambda$ can be repeated

#### solve for $x$

Back substitute $\lambda$
