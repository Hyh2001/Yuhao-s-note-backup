#calculus/differentiation 
Let $f$ be a function that satisfies the following three hypotheses:

1. $f$ is continuous on the closed interval $[a,b]$
2. $f$ is differentiable on the open interval $(a,b)$
3. $f(a) = f(b)$
   Then there is a number $c$ in $(a,b)$ such that $f^{'}(c) = 0$

### proof

#### Case 1. $f(x) = k$

Then $f^{'}(x) = 0$, so the number $c$ can be taken to be any number in $(a,b)$.

#### Case 2.$f(x) > f(a)$ for some $x$ in $(a,b)$

By [[extreme value theorem]], we can get that there must a [[local maximum]] at $c$ in $(a,b)$ for $f(a) = f(b)$, and at the local maximum $f^{'}(c) = 0$

#### Case 3.$f(x) < f(a)$ for some $x$ in $(a,b)$

By [[extreme value theorem]], we can get that there must a [[local minimum]] at $c$ in $(a,b)$ for $f(a) = f(b)$, and at the local maximum $f^{'}(c) = 0$
