Taylor series is a special type of [[power series]] where the coefficients $c_{n}=\frac{f^{(n)}(a)}{n!}$. The equations is:: 
$$\begin{aligned}
f (x) & =\sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n !}(x-a)^n \\
& =f (a)+\frac{f^{\prime}(a)}{1 !}(x-a)+\frac{f^{\prime \prime}(a)}{2 !}(x-a)^2+\frac{f^{\prime \prime \prime}(a)}{3 !}(x-a)^3+\cdots
\end{aligned}$$
and we call it as Taylor series of the function at $a$ 
([Stewart, 2016, p. 760](zotero://select/library/items/BIS3IDTH)) ([pdf](zotero://open-pdf/library/items/BQP5L6YK?page=792&annotation=6CJR8FAL))
When $a=0$, the series becomes the [[Maclaurin series]]. 

# derivation 
We denote the function as $f (x) = c_{0}+c_{1}(x-a)+c_{2}(x-a)^{2}+c_{3}(x-a)^{3}+c_{4}(x-a)^{4}+\ldots$ for $|x-a|<R$ 
It is obvious that if we take $x=a$, then $f(a)=c_{0}$. 
We then [[differentiate]] the series and we get $f^{\prime}(x)=c_{1}+2c_{2}(x-a)+3c_{3}(x-a)^{2}+4c_{4}(x-a)^{3}+\ldots$ and it is also obvious that when $x=a$, $f^{'}(a)=c_{1}$ 
If we iteratively differentiate both sides, we will find that finally $c_{n}=\frac{f^{n}(a)}{n!}$ 
([Stewart, 2016, p. 759](zotero://select/library/items/BIS3IDTH)) ([pdf](zotero://open-pdf/library/items/BQP5L6YK?page=791&annotation=K9NYQYD4))