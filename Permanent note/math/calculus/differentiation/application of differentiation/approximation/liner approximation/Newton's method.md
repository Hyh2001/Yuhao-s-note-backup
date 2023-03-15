It is **second** [[order of convergence]] [[iterative method]] . It is a special **[[fixed point iteration]]** method. ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=58&annotation=MM9Y6UZ4))
# derivation of the method 
We can approximate a [[function]] $f(x)$ at $x_k$ by using the first order [[Taylor polynomial]]. $p (x) = f(x_k)+f^{'}(x_k)(x-x_k)$. To find a root for $x$, we can solve $p (x) =0$ instead: $x_{k+1}=x_{k}-\frac{f (x_{k})}{f^{'}(x_{k})}= \varphi(x)$  
([pdf](zotero://open-pdf/library/items/X3UESHXG?page=59&annotation=7JE7QTZP))
# steps <!--SR:!2023-03-16,4,270!2023-03-16,3,252-->

1. We guess an approximation called $x_1$
2. Find the tangent line of the curve at $x_1$
3. find the x-intersect of the tangent line
4. Repeat the above steps using the intersect $x_2$
5. the answer iteratively will be $x_{n+1} = x_n - \frac{f(x_n)}{f^{'}(x_n)}$
6. the final answer is $lim_{n \to \infty} x_n = r$

## [[order of convergence]] 
Newton's method is at least a quadratic convergence method. 
We can see it by differentiate $\varphi(x)$ 
$\varphi^{\prime}(x) = \frac{f(x)f^{''}(x)}{[f^{'}(x)]^2}$
$f (x) = 0$ for $x\to x^{*}$. Then if $f^{'}(x^{*})\neq 0$, the method converges locally ([[local convergence]] ) with order $2$ 
([pdf](zotero://open-pdf/library/items/X3UESHXG?page=67&annotation=QW7VQ93P))
### when the convergence loses its priority
When $f^{\prime}(x)=0$
# problems of the method 
1.  $f^{'}(x_1)$ is close to $0$ which makes $x_2$ to be a bad choice
	solution: Chose a better $x_1$
1. We need to know $f^{'}(x)$ in order to use this method 
	solution: use the [[Newton's secant method]] or [[secant method]] 

