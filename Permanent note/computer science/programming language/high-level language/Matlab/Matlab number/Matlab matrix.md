## size of a [[matrix]] or an [[array]]

```matlab
a = size(x) % a is an array [row, column] 
[r,c] = size(x) % r and c are row length and column length 
len = length(x) % this will return the length of an array 
```

## representation of matrix

```matlab
X = [ 1 2 3 4 5 6; 7 8 9 10 11 12]
X = [ 1 2 3 4
		5 6 7 8] % is equal to above
```

### empty matrix

```matlab
x = []
% accessing part of a matrix
```
### with known number of  elements 
```matlab 
linspace(first, last, number_of_elements)
```
### with random elements 
```matlab 
x = rand(n)  % build n*n matrix with random variables
y = rand(m,n) % build m*n matrix with random variables
```
### With zeros 
```matlab 
x = zeros(m,n)  %create a m*n matrix with zeros
```
### With ones
```matlab 
x = ones(m,n) %create a m*n matrix with ones 
```
## Slicing

```
X(a,b) % a specify rows and b specify columns
X(end-1,2) % end specifies the last row

```

### access multiple parts

```matlab
X(a,[b,c]) % see column b and c
X(a,b:c) % see columns from b to c
X(a,:) % see all the columns
X(1,2:end) % end means the last row or column
```

### assign values to undefined parts

Will keep the value and fill other places with zeros


## Matrix calculations
### Maximum number of an array 
```matlab
a = max(v)   % get the biggest number in v
[a,id] = max(v) % a is the biggest number and id is the index of it
```
### Matrix combination

Should be in the shape of rectangles after combination

```
[A1 A2 A3] % along x direction
[A1;A2;A3] % along y direction
```

### Transpose

```matlab
A’
```
### Element-wise multiplication
```matlab
c = a .* b %a and b are two arrays
```
## [[complex number]] 

```matlab
x = 3 +4j or x = 3 + 4i
```

# [[ Matlab operator]]


