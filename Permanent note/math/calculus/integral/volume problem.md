#calculus/integral

let $S$ be a solid that lies between $x=a$ and $x=b$. If the cross-sectional area of $S$ in the plane $p_x$, through $x$ and perpendicular to the $x$-axis, is $A(x)$, where $A$ is a continuous function, then the *volume* of $S$ is  
$V = \lim_{n \to \infty}\sum_{i=1}^n A(x_i^*)\delta x = \int_a^bA(x)dx$  
核心思路为两条曲线的差值

## for cylindrical shell (obtained by rotating about the axis)

思路：大圆环减去小圆环  
​$V = \pi (r_2+r_1)h (r_2-r_1)$( r is independent with x)  
$V = \int_a^b 2\pi xf(x)dx$, where $0 \leq a < b$ ( r is dependent with x)

‍
