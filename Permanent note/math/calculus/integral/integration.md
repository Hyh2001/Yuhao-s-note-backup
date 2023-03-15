#calculus/integral 

Integration is mainly used in some problems that need to find the area of a region bounded by a curve.(It is find the Riemann sum[^1] of infinite small areas) It can be used in real problems like area problem[^2], volume problem[^3], average value of a function[^4] distance problem. integral[^5]s are the outcomes of integration. Integration is the inverse process of differential[^7]. With the fundamental theorem of calculus[^8], we can find the value of a definite integral[^13] by using its antiderivative[^12].  
We can have several methods to find antiderivative[^12]s of many functions. They include:

1. substitution rule[^14]
2. integration by parts[^15]
3. trigonometric integration[^16]

‍

[^1]: # Riemann sum

    ​#calculus/integral#​

    ​#todo#​


[^2]: # area problem

    ​#calculus/integral#​

    The *area* $A$ of the region $S$ that lies under the graph of the continuous function $f$ is the limit of the sum of the areas of approximating rectangles:
    $A = lim_{n \to \infty} R_n = lim_{n \to \infty}[f(x_1) \delta x + f(x_2) \delta x + ... + f(x_n) \delta x]$

    ## area bounded by two curves

    The area $A$ of the region bounded by the curves $y=f(x),y=g(x)$, and the lines $x=a,x=b$,where $f$ and $g$ are [[continuous on an interval]] and $f(x) \geq g(x)$ for all $x$ in $[a,b]$, is  
    ​$A = \int_a^b[f(x)-g(x)]dx$  
    The area bounded between two curves is as follow.  
    ​$A = \int_a^b|f(x)-g(x)|dx$  
    note that this formula do not care about which curve is at the top


[^3]: # volume problem

    ​#calculus/integral#​

    # method

    let $S$ be a solid that lies between $x=a$ and $x=b$. If the cross-sectional area of $S$ in the plane $p_x$, through $x$ and perpendicular to the $x$-axis, is $A(x)$, where $A$ is a continuous function, then the *volume* of $S$ is  
    ​$V = \lim_{n \to \infty}\sum_{i=1}^n A(x_i^*)\delta x = \int_a^bA(x)dx$  
    核心思路为两条曲线的差值

    ## for cylindrical shell (obtained by rotating about the axis)

    思路：大圆环减去小圆环  
    ​$V = \pi (r_2+r_1)h (r_2-r_1)$( r is independent with x)  
    ​$V = \int_a^b 2\pi xf(x)dx$, where $0 \leq a < b$ ( r is dependent with x)

    ‍


[^4]: # average value of a function

    We can find the average value of a function by [[integration]], using the formula below:
    $f_{avg} = \frac{1}{b-a}\int_a^bf(x)dx$
    Also If we denote $f(c) = f_{avg}$
    we can have the [[mean value theorem of integration]]


[^5]: # integral

    ​#calculus/integral#​

    Integral is the result of a mathematical integration[^6]. There are two types of integrals. The first type is definite integral[^13] and the second is indefinite integral[^17].


[^6]: # integration

    ​#calculus/integral#​

    Integration is mainly used in some problems that need to find the area of a region bounded by a curve.(It is find the Riemann sum[^1] of infinite small areas) It can be used in real problems like area problem[^2], volume problem[^3], average value of a function[^4] distance problem. integral[^5]s are the outcomes of integration. Integration is the inverse process of differential[^7]. With the fundamental theorem of calculus[^8], we can find the value of a definite integral[^13] by using its antiderivative[^12].  
    We can have several methods to find antiderivative[^12]s of many functions. They include:

    1. substitution rule[^14]
    2. integration by parts[^15]
    3. trigonometric integration[^16]

    ‍


[^7]: # differential

    # definition

    differential of $y$ can be $dy = f^{'}(x)dx$
    A ratio of two infinitesimals


[^8]: # the fundamental theorem of calculus

    ​#calculus/integral#​

    # The fundamental theorem of calculus, 1

    If $f$ is continuous on $[a,b]$, then the function $g$ defined by
    $g(x) = \int_a^x f(t) dt$     $a \leq x \leq b$
    Is continuous on $[a,b]$ and differentiable on $(a,b)$, and $g^{'}(x) =f (x)$

    #### proof

    If $x$ and $x+h$ are in $(a,b)$, then  
    ​$g(x+h) - g(x) = \int_a^{x+h}f(t)dt - \int_a^xf(t)dt = (\int_a^xf(t)dt + \int_x^{x+h}f(t)dt) - \int_a^xf(t)dt = \int_x^{x+h}f(t)dt$  
    assume $h \neq 0$,  
    ​$\frac{g(x+h)-g(x)}{h} = \frac{1}{h}\int_x^{x+h}f(t)dt$  
    by the extreme value theorem[^9], for $f$ continuous on $[x,x+h]$, there are always absolute maximum[^10] $f(u) = m$ and absolute minimum[^11] $f(v) = M$  
    For $f$, we have:  
    ​$f(u)h \leq \int_x^{x+h}f(t)dt \leq f(v)h$  
    we get:  
    ​$f(u) \leq \frac{g(x+h)-g(x)}{h} \leq f(v)$  
    Let $h \to 0$  
    we can get $\lim_{h \to 0} f(u) = f(x)$, $\lim_{h \to 0} f(v) = f(x)$  
    thus,  
    ​$lim_{h \to 0}\frac{g(x+h)-g(x)}{h} = g^{'}(x) =f(x)$  

    # The fundamental theorem of calculus, 2

    If $f$ is continuous on $[a,b]$, then  
    ​$\int_a^bf(x)dx = F(b) - F(a)$  
    where $F$ is any antiderivative[^12] of $f$, that is, a function such that $F^{'} =f$  

    #### proof

    let $g(x) = \int_a^x f(t)dt$, then we will have
    $F(x) = g(x) + C$ for $a &lt; x &lt; b$
    For $F$ and $g$ are continuous, the relation above is true for $x$ in $[a,b]$
    Let $x = a$, then $g(a) = \int_a^af(t)dt = 0$
    $F(b) - F(a) = g(b) - g(a) = g(b) = \int_a^bf(t)dt$


[^9]: # the extreme value theorem

    # definition

    If $f$ is continuous on a closed interval $[a,b]$,then $f$ attains an absolute maximum value $f(c)$ and an absolute minimum value $f(d)$ at some numbers $c$ and $d$ in $[a,b]$


[^10]: # absolute maximum

    # definition

    Let $c$ be a number in the domain $D$ of a function $f$. Then $f(c)$ is the:
    *absolute maximum* value of $f$ on $D$ if $f(c) \geq f(x)$ for all $x$ in $D$


[^11]: # absolute minimum

    # definition

    Let $c$ be a number in the domain $D$ of a function $f$. Then $f(c)$ is the:
    *absolute minimum* value of $f$ on $D$ if $f(c) \leq f(x)$ for all $x$ in $D$


[^12]: # antiderivative

    A function $F$ is called an antiderivative of $f$ on an interval $I$ if $F^{'}(x) = f(x)$ for all $x$ in $I$

    # general [[antiderivative]]

    If $F$ is an antiderivative of $f$ on an interval $I$, then the most general antiderivative of $f$ on $I$ is $F(x) + C$, $C$ is an arbitrary constant.


[^13]: # definite integral

    ​#calculus/integral#​

    If f is a function defined for $a &lt; x &lt; b$, we divide the interval $[a,b]$ into $n$ subintervals of equal width $\delta x = (b-a)/n$. We let $x_0 (=a),x_1,x_2,...,x_n(-b)$ be the endpoints of these subintervals and we let $x_1^*, x_2^*, . . . , x_n^*$ be any sample points in these subintervals, so $xi^*$ lies in the $i$th subinterval $[x_{i-1},x_i]$. Then the *definite integral of ​*​*$f$*​*​ from ​*​*$a$*​*​ to ​*​*$b$* is
    $\int^{b}_{a} f(x)dx = lim_{n \to \infty}\sum _{i=1}^{n}f(x_i*)\delta x$
    provided that this limit exists and gives the same value for all possible choices of sample points. If it does exist, we say that $f$ ($f(x)$ is called the *integrand*) is [[Integrable]] on $[a,b]$($a$ is called the *lower limit* and $b$ is called the *upper limit*).

    # easy form

    Because for randomly choosing sample points are hard, we directly choose the endpoints of each interval as the endpoint. We let $x_i^* = x_i$ Which $x_i$ is the end points of the intervals. Then
    $\int_b^a f(x)dx = lim_{n \to \infty}\sum^n_{i=1}f(x_i)\delta x$
    Where $\delta x = \frac{b-a}{n}$ and $x_i = a + i\delta x$

    # The Midpoint rule

    When we need to find an approximation to an [[integral]] , we can use [[the midpoint rule]].

    # precise definition

    The precise definition of definite integral is as follow. ==Why we need this precise definition?==
    For every number $\epsilon &gt; 0$ there is an integer $N$ such that,
    $|\int^{b}_{a} f(x)dx - \sum^{n}_{i=1}f(x_i^*)\delta x| &lt; \epsilon$
    for every integer $n&gt;N$ and for every choice of $x_i^*$ in $[x_{i-1},x_i]$

    # properties of definite integral

    There are several properties of definite integral, and they are as follow.

    1. $\int_b^a f(x)dx = -\int_a^bf(x)dx$
    2. $\int_a^a f(x)dx = 0$
    3. $\int_a^b c dx = c(b-a)$
    4. $\int_a^b [f(x)+g(x)]dx = \int_a^bf(x)dx + \int^b_ag(x)dx$
    5. $\int_a^b cf(x)dx = c\int^b_a f(x)dx$
    6. $\int_a^b[f(x) -g(x)]dx = \int_a^b f(x)dx - \int_a^bg(x)dx$
    7. If $f(x) \geq 0$ for $a \leq x \leq b$, then $\int_a^bf(x) dx \geq 0$
    8. If $f(x) \geq g(x)$ for $a \leq x \leq b$, then $\int_a^bf(x)dx \geq \int_a^bg(x)dx$
    9. If $m \leq f(x) \leq M$ for $a \leq x \leq b$, then
       $m(b-a) \leq \int_a^bf(x)dx \leq M(b-a)$


[^14]: # substitution rule

    ​#calculus/integral#​

    If $u = g(x)$ is a differentiable function whose range is an interval $I$ and $f$ is continuous on $I$, then
    $\int f(g(x))g^{'}(x)dx = \int f(u)du$

    #### proof

    Let $u = g(x)$, then $du = g^{'}(x)dx$


[^15]: # integration by parts

    ​#calculus/integral#​

    This method is corresponding to the product rule( see [[derivative rules]] ).
    $\frac{d}{dx}[f(x)g(x)] = f(x)g^{'}(x) + f^{'}(x)g(x)$
    [[integral]] both side
    $f(x)g(x) = \int f(x)g^{'}(x) dx + \int f^{'}(x)g(x) dx$

    # for [[definite integral]]

    $f(x)g(x)|^a_b = \int_b^a f(x)g^{'}(x) dx + \int_b^a f^{'}(x)g(x) dx$


[^16]: # trigonometric integration

    ​#calculus/integral#​

    There are several methods to integrate trigonometric functions

    # for sin(x)cos(x) like

    $\int sin^m(x)cos^n(x)dx$

    1. if $n = 2k +1$
       $\int sin^m(x)cos^{2k+1}(x)dx = \int sin^m(x)cos^{2k}(x)cos(x)dx = \int sin^m(x)(1-sin^2(x))^kcos(x)dx$, then substitute $u =sin(x)$
    2. if m = 2k + 1
       $\int sin^{2k+1}(x)cos^n(x)dx = \int sin^{2k}(x)cos^n(x)sin(x)dx = \int (1-cos^2(x))^kcos^n(x)sin(x)dx$, then substitute $u =cos(x)$
    3. both n and m are even
       use $sin(x)cos(x) = \frac{1}{2}sin(2x)$

    # for tan(x)sec(x) like

    1. n is even
       $\int tan^m(x)sec^{2k}(x) dx = \int tan^m(x)sec^{2k-2}(x) sec^{2}(x)dx = \int tan^{m}x(1+tan^2(x))^{k-1}sec^2(x) dx$
    2. m is odd
       $\int tan^{2k+1}(x)sec^{n}(x) dx = \int tan^{2k}(x)sec^{n-1}(x) sec(x)tan(x)dx = \int (sec^2(x)-1)^k sec^{n-1}(x)sec(x)tan(x) dx$


[^17]: # indefinite integral

    ​#calculus/integral#​

    Indefinite integral denotes the connection between a function and its antiderivative[^12] , it is a [[function]] (or a family of functions)  
    ​$\int f(x)dx = F(x)$ and $F^{'}(x) = f(x)$  

    # calculation laws

    The calculation laws of indefinite integral is as follow

    1. $\int cf(x) dx = c\int f(x) dx$
    2. $\int kdx = kx + C$
    3. $\int x^n dx = \frac{x^{n+1}}{n+1} + C$
    4. $\int [f(x)+g(x)]dx = \int f(x)dx + \int g(x)dx$
    5. $\int_a^b cf(x)dx = c\int^b_a f(x)dx$
    6. $\int \frac{1}{x} dx = ln|x| + C$
    7. $\int e^x dx = e^x + C$
    8. $\int b^x dx = \frac{b^x}{In b} + C$
    9. $\int sin(x) dx = -cos(x) + C$
    10. $\int cos(x) dx = sin(x) + C$
    11. $\int sec^2(x) dx = tan(x) + C$
    12. $\int csc^2(x) dx = -cot(x) + C$
    13. $\int sec(x)tan(x) dx = sec(x) + C$
    14. $\int csc(x)cot(x) dx = -csc(x) + C$
    15. $\int \frac{1}{x^2+1} dx = tan^{-1}x + C$
    16. $\int \frac{1}{\sqrt{1 - x^2}} dx = sin^{-1}x + C$
    17. $\int sinh(x) dx = cosh(x) + C$
    18. $\int cosh(x) dx = sinh(x) + C$
    19. $\int tan(x)dx = ln|sec(x)| +C$​
    20. If $f(-x) = f(x)$, then $\int^a_{-a}f(x)dx = 2\int_0^af(x)dx$
    21. If f(-x) = -f(x), then $\int^a_af(x)dx = 0$

    ‍
