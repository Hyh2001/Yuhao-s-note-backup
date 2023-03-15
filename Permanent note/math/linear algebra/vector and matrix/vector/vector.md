#linear_algebra #calculus #differential_equation 
It is the special objects that can be added together and multiplied by scalars to produce another object of the same kind. It is in a form of a **finite** **ordered** list of numbers or unknowns. Same vector can have different endpoints, they only need to have the same magnitude and direction. There are two types of vectors. [[column vector]]s and [[row vector]]s
## real life counterparts:

1. Audio signals
2. $R^n$
3. [[array]] (used in [[machine learning]])
4. place of a point in a space

## representation of vector

1. a line with directions in the space
2. use coordinates in $n$-dimensional spaces

# properties of vector 
1. [[norm]]
# calculation law:

## vector addition

Vector addition obeys[[ parallelogram rule]]

In coordinates form, $\vec{a} + \vec{b} = (a_1 + b_1, a_2 + b_2,...a_n+b_n)$ where $a_1,a_2,... b_1,b_2,..$ are coordinates of $\vec{a}, \vec{b}$

## vector multiplication

### by scalars

$c \cdot \vec{a} = c\vec{a}$  

In coordinates form, $c\vec{a} = (ca_1 , ca_2 ,...,ca_n)$ where $a_1,a_2,...$ are coordinates of $\vec{a}$
#### [[parallel vector]]
Two vectors $m,n$ are parallel to each other if there exists a real number $a$ such that $\vec{m} = a\vec{n}$
### [[dot product]]

$v \cdot w = v_1w_1 + v_2w_2$  

### [[cross product]]

## vector difference 
$V -U$ is called the difference of $V$ and $U$

# special vectors:

1. [[unit vector]] : For arbitrary vectors, we can construct a unit vector by $u = v/||v||$  
2. [[zero vector]]

# programming implementation of vector

## Julia

```julia
a = [1 -2 4 8.1 2^0.5] # 1 * 5 matrix 
b = [1, -2, 4, 8.1, 2^0.5] # 5 * 1 matrix 
c = [1; -2; 4; 8.1; 2^0.5] # another representation of 5 * 1 matrix
```

## 

‍

‍

1. ‍
2. [ROB_101_December_2021_Grizzle - Excerpt of: ROB_101_December_2021_Grizzle, p27](lt://open/Awf0qGUlxEaKidzJdZ0Qtw)
3. [mathematical analysis - Excerpt of: Second Year Calculus From Celestial Mechanics t... (z-lib.org), p17](lt://open/5-xhoqEwDEyWwLPg5Yg6bA)
