#calculus/differentiation 
Let $f$ be a function that satisfies the following hypotheses:
1. $f$ is [[continuity|continuous]] on the [[closed interval]]  $[a,b]$
2. $f$ is [[differentiable]]  on the open interval $(a,b)$
   Then there is a number $c$ in $(a,b)$ such that
   $f^{'}(c) = \frac{f(b) -f(a)}{b - a}$

### proof

we write line AB as $y = f(a) + \frac{f(b) -f(a)}{b -a} (x-a)$
we let $h(x) = f(x) - f(a) - \frac{f(b) -f(a)}{b -a} (x-a)$
$h(x)$ satisfies [[Rolle‘s theorem]] 
and we know that there is a $c$ that $h^{'}(c) = f^{'}(c) - \frac{f(b) -f(a)}{b -a} = 0$
then $f^{'}(c) = \frac{f(b) -f(a)}{b -a}$

### theorem 1

If $f^{'}(c)$ for all $x$ in an interval $(a,b)$, then $f$ is constant on $(a,b)$

### corollary of theorem 1

If $f^{'}(x) = g^{'}(x)$ for all $x$ in an interval $(a,b)$ then $f - g$ is constant on $(a,b)$; that is, $f(x) = g(x) + c$ where $c$ is a constant.
