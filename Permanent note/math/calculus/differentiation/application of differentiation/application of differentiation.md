#calculus/differentiation #review 
# areas
1. optimization problems

## absolute maximum and absolute minimum

Let $c$ be a number in the domain $D$ of a function $f$. Then $f(c)$ is the:
*absolute maximum* value of $f$on $D$ if$f(c) \geq f(x)$ for all $x$ in $D$
*absolute minimum* value of $f$ on $D$ if $f(c) \leq f(x)$ for all $x$ in $D$

### how to find them(closed interval method)

1. Find the values of $f$ at the critical numbers of $f$ in $[a,b]$.
2. Find the values of f at the endpoints of the interval.
3. The largest of the values from Steps 1 and 2 is the absolute maximum value; the smallest of these values is the absolute minimum value.

## local maximum and local minimum

The number $f(c)$is a
*local maximum* value of f if $f(c) \geq f(x)$ when $x$ is near $c$
*local minimum* value of f if $f(c) \leq f(x)$ when $x$ is near $c$

## the extreme value theorem

If $f$ is continuous on a closed interval $[a,b]$,then $f$ attains an absolute maximum value $f(c)$ and an absolute minimum value $f(d)$ at some numbers $c$ and $d$ in $[a,b]$

## fermat's theorem

If $f$ has a local maximum or minimum at $c$, and if $f^{'}(c)$ exists, then $f^{'}(c) = 0$

### proof

$f^{'}(c) = \frac{f(h+c) - f(c)}{h}$
for $c$ is a local maximum or minimum $f(c +h) -f(c) \leq 0$
let $h &gt; 0$
$lim_{h \to 0^+}\frac{f(h+c) - f(c)}{h} \leq 0$
let $h&lt;0$
$lim_{h \to 0^-}\frac{f(h+c) - f(c)}{h} \geq 0$
for they are all true
$f^{'}(c) = \frac{f(h+c) - f(c)}{h} = 0$

## critical number

A critical number of a function $f$ is a number $c$ in the domain of $f$ such that either $f^{'}(c) = 0$ or $f^{'}(c)$ does not exist
<font color="00FF00" size="3">critical number includes local maximum and local minimum but not only them</font>

## Rolle's theorem

Let $f$ be a function that satisfies the following three hypotheses:

1. $f$ is continuous on the closed interval $[a,b]$
2. $f$ is differentiable on the open interval $(a,b)$
3. $f(a) = f(b)$
   Then there is a number $c$ in $(a,b)$ such that $f^{'}(c) = 0$

### proof

#### Case 1. $f(x) = k$

Then $f^{'}(x) = 0$, so the number $c$ can be taken to be any number in $(a,b)$.

#### Case 2.$f(x) &gt; f(a)$ for some $x$ in $(a,b)$

By extreme value theorem, we can get that there must a local maximum at $c$ in $(a,b)$ for $f(a) = f(b)$, and at the local maximum $f^{'}(c) = 0$

#### Case 3.$f(x) &lt; f(a)$ for some $x$ in $(a,b)$

By extreme value theorem, we can get that there must a local minimum at $c$ in $(a,b)$ for $f(a) = f(b)$, and at the local maximum $f^{'}(c) = 0$

## mean value theorem

Let $f$ be a function that satisfies the following hypotheses:

1. $f$ is continuous on the closed interval $[a,b]$
2. $f$ is differentiable on the open interval $(a,b)$
   Then there is a number $c$ in $(a,b)$ such that
   $f^{'}(c) = \frac{f(b) -f(a)}{b - a}$

### proof

we write line AB as $y = f(a) + \frac{f(b) -f(a)}{b -a} (x-a)$
we let $h(x) = f(x) - f(a) - \frac{f(b) -f(a)}{b -a} (x-a)$
$h(x)$ satisfies Rolle's theorem
and we know that there is a $c$ that $h^{'}(c) = f^{'}(c) - \frac{f(b) -f(a)}{b -a} = 0$
then $f^{'}(c) = \frac{f(b) -f(a)}{b -a}$

### theorem 1

If $f^{'}(c)$ for all $x$ in an interval $(a,b)$, then $f$ is constant on $(a,b)$

### corollary of theorem 1

If $f^{'}(x) = g^{'}(x)$ for all $x$ in an interval $(a,b)$ then $f - g$ is constant on $(a,b)$; that is, $f(x) = g(x) + c$ where $c$ is a constant.
