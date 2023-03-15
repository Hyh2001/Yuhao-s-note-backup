#linear_algebra 

A $m,n$ tuple according to a rectangle scheme of m rows and n columns. Each row or column is a vector[^1]. The element of each entry is noted as $a_{ij}$ where it indicates $i$-th row and $j$-th column.   
​$\begin {bmatrix} 0 & 1 & 1\\ 0 & 0 & 1 \end{bmatrix}$  

A matrix can be used to represent a system of [[linear equation]] s 
$\begin{matrix} x_1 +x_2 = 4 \\ 2x_1 - x_2 = -1 \end{matrix} = \begin{bmatrix} 1 & 1 \\ 2 & -1 \end{bmatrix} \begin{bmatrix}x_1 \\ x_2 \end{bmatrix}$
## Features of matrices 
### [[diagonal]]
## calculations

### addition

$A + B = a_{ij} + b_{ij}$ for each entries

### [[matrix multiplication]]

### [[transpose]]

## special matrices

1.  [[square matrix]]
2.  [[Identity matrix]]
3.  [[diagonal matrix]]
4. [[upper-triangular matrix]] ]
5. [[lower-triangular matrix]] 
6. [[symmetric matrix]] 
7. [[skew-symmetric matrix]] 
8. [[permutation matrix]] 
# programming representation 

## julia representation of matrix

1. build a matrix or a vector

```julia
A = [ 1.2 -2.6 11.7; 3.1 11/7 0] # 2 * 3 matrix
B = [1 1 1] # a 1 * 3 matrix
C = [1, 1, 1] # a 3 * 1 matrix
D = [1; 1; 1] # a 3 * 1 matrix
A = randn (m,n) # build a random matrix
```

2. matrix indexing

    ```julia
    A[x,y] # this will return the x-th row and y-th column entry of the matrix
    # : selects all elements along that dimension 
    # warning: 抽取向量时永远返回列向量无论这个向量在原矩阵中是否是列向量
    A[:,3]  
    A[2,:]
    # stacks all the columns as a vector
    A[:]
    # stacks all the rows as a vector
    A'[:]


    ```
3. test whether matrix are equal

```julia
A == B
```

## latex matrix

```latex
$\begin{array}{l} a & b\\ c& d \end{array}$
$\begin{vmatrix} a & b\\ c& d \end{vmatrix}$
$g(\theta) = \begin{bmatrix} g_1(\theta_1,...\theta_n) \\ . \\. \\. \\ g_k(\theta_1,...,\theta_n)\end{bmatrix}$
```

## matlab matrix representation
See [[Matlab matrix]]
## python matrix representation
