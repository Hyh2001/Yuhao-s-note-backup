#calculus/integral#

If f is a function defined for $a &lt; x &lt; b$, we divide the interval $[a,b]$ into $n$ subintervals of equal width $\delta x = (b-a)/n$. We let $x_0 (=a),x_1,x_2,...,x_n(-b)$ be the endpoints of these subintervals and we let $x_1^*, x_2^*, . . . , x_n^*$ be any sample points in these subintervals, so $xi^*$ lies in the $i$th subinterval $[x_{i-1},x_i]$. Then the *definite integral of ​*​*$f$*​*​ from ​*​*$a$*​*​ to ​*​*$b$* is
$\int^{b}_{a} f(x)dx = lim_{n \to \infty}\sum _{i=1}^{n}f(x_i*)\delta x$
provided that this limit exists and gives the same value for all possible choices of sample points. If it does exist, we say that $f$ ($f(x)$ is called the *integrand*) is [[Integrable]] on $[a,b]$($a$ is called the *lower limit* and $b$ is called the *upper limit*).

# precise definition
The precise definition of definite integral is as follow. ==Why we need this precise definition?==
For every number $\epsilon &gt; 0$ there is an integer $N$ such that,
$|\int^{b}_{a} f(x)dx - \sum^{n}_{i=1}f(x_i^*)\delta x| &lt; \epsilon$
for every integer $n&gt;N$ and for every choice of $x_i^*$ in $[x_{i-1},x_i]$

# easy form
Because for randomly choosing sample points are hard, we directly choose the endpoints of each interval as the endpoint. We let $x_i^* = x_i$ Which $x_i$ is the end points of the intervals. Then
$\int_b^a f(x)dx = lim_{n \to \infty}\sum^n_{i=1}f(x_i)\delta x$
Where $\delta x = \frac{b-a}{n}$ and $x_i = a + i\delta x$

# approximation to definite integral
When we need to find an approximation to definite integral, we can use [[the midpoint rule]].


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
