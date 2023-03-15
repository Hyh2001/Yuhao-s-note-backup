​ #calculus/integral #todo #review 

# The fundamental theorem of calculus, 1

If $f$ is continuous on $[a,b]$, then the function $g$ defined by
$g(x) = \int_a^x f(t) dt$     $a \leq x \leq b$
Is continuous on $[a,b]$ and differentiable on $(a,b)$, and $g^{'}(x) =f (x)$

#### proof

If $x$ and $x+h$ are in $(a,b)$, then  
​$g(x+h) - g(x) = \int_a^{x+h}f(t)dt - \int_a^xf(t)dt = (\int_a^xf(t)dt + \int_x^{x+h}f(t)dt) - \int_a^xf(t)dt = \int_x^{x+h}f(t)dt$  
assume $h \neq 0$,  
​$\frac{g(x+h)-g(x)}{h} = \frac{1}{h}\int_x^{x+h}f(t)dt$  
by the extreme value theorem[^1], for $f$ continuous on $[x,x+h]$, there are always absolute maximum[^2] $f(u) = m$ and absolute minimum[^3] $f(v) = M$  
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
where $F$ is any antiderivative[^4] of $f$, that is, a function such that $F^{'} =f$  

#### proof

let $g(x) = \int_a^x f(t)dt$, then we will have
$F(x) = g(x) + C$ for $a &lt; x &lt; b$
For $F$ and $g$ are continuous, the relation above is true for $x$ in $[a,b]$
Let $x = a$, then $g(a) = \int_a^af(t)dt = 0$
$F(b) - F(a) = g(b) - g(a) = g(b) = \int_a^bf(t)dt$

