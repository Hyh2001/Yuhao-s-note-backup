Fixed point iteration is an [[iterative method]] which is used to find a root for a function $f(x)$. We transfer the problem to find **[[fixed point]]** for a function $\varphi(x)$ (this function is called the iterative function and it is not **unique** on $[a,b]$. ) ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=11&annotation=8SANICJJ)) ([Ascher 和 Greif, 2011, p. 62](zotero://select/library/items/HJK4ZQRP)) ([pdf](zotero://open-pdf/library/items/FSDKG9DD?page=62&annotation=ZIICK7MB))

# algorithm 
1. we give an initial guess as $x_{0}\in [a,b]$ 
2. we calculate $x_{1} = \varphi(x_0)$, if $x_{1}= x_{0}$ then $x_{1}$ is a [[root]]. Otherwise continue 
3. we calculate $x_{2} = \varphi(x_1)$, if $x_{2}= x_{0}$ then $x_{2}$ is a root. Otherwise continue 
4. ....
5. Finally we meet the stopping criterion and finish the iteration. 
([pdf](zotero://open-pdf/library/items/X3UESHXG?page=12&annotation=K42I6TCL)) ([Ascher 和 Greif, 2011, p. 63](zotero://select/library/items/HJK4ZQRP)) ([pdf](zotero://open-pdf/library/items/FSDKG9DD?page=63&annotation=EVUG73W4))
## stopping criterion 
We can use several stopping criterions. 
1. [[absolute error]] approach: $|x_{k+1} -x_{k}|<\epsilon$ 
2. [[relative error]] approach: $|x_{k+1} -x_{k}|<\epsilon{x_k}$
3. absolute or relative error: $|x_{k+1} -x_{k}|<\epsilon(1+|x_{k}|)$ 
4. function value: $|f (x_{k})| < \epsilon$ 
$\epsilon$ is the [[error bound]] given by us ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=31&annotation=KZ7V8H87))
## number of iterations 
We can find a positive integer $K$ such that $|x_{k} - x^{*}| < \epsilon$, $\forall k >K$ ($\epsilon$ is the stopping criteria). 
$K = \lceil{}\frac{ln|x_{1}-x_{0}|-ln (\epsilon (1-L))}{ln (\frac{1}{L})}\rceil$ where $\lceil m \rceil$ denotes the smallest integer greater than or equal to $m$. ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=26&annotation=TPUWQ7GR))
### proof 
If we take $k$ big enough than we can have $\epsilon \geq \frac{L^k}{1-L}|x_1-x_0|$ (right part of the inequality is the error defined in global convergence)
We take logarithm of both sides and we get $k \geq \frac{ln|x_{1}-x_{0}|-ln (\epsilon (1-L))}{ln (\frac{1}{L})}$ ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=27&annotation=6W7PYEYA))

# [[fixed point iteration - global convergence]]
# [[fixed point iteration - local convergence]]


# [[order of convergence]] 
We can derive the order of convergence the method as follow: 
$\frac{e_{k+1}}{e_{k}} \to \varphi^{'}(x^{*})$ because $x_{k+1}-x^{*} = \varphi^{'}(\xi)(x_{k}-x^{*})$  (using [[mean value theorem]]). If $0<|\varphi^{'}(\xi)|<1$ then the method converges linearly, if $\varphi^{'}(\xi) = 0$ then the method converges superlinearly. 

## accelerate the order of convergence 
### method 1
we can construct a new function :: $\phi = \frac{1}{1-L}[\varphi(x)-Lx]$ to replace the original $\varphi(x)$ where $L = \varphi^{\prime}(x)$  ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=52&annotation=XQH9HWV4))
proof: 
We can proof $\varphi(x_{k})-\varphi(x^{*}) = \varphi^{'}(\xi)(x_{k}-x^{*})$ by using [[mean value theorem]]. we take [[limit]] of it, we get: 
$\lim_{k\to \infty} \frac{\varphi (x_{k})-x^{*}}{x_{k}-x^{*}} = \varphi^{'}(x^{*})$. (It is because that with $x_k$ approaches $x^{*}$, and  $\varphi(\xi)$ is between $\varphi(x_k)$ and $\varphi(x^{*})$, $\xi \to x^{*}$)
We assume $\varphi\left(x_k\right)-x^* \approx L\left(x_k-x^*\right), \quad \forall x_k \in \Delta^{\prime},$ 
where $L \approx \varphi^{\prime}\left(x^*\right)$ and $\Delta^{\prime}$ is a neighborhood of $x^*$ contained in
$\Delta$. ($\Delta$ is the domain in which $x_0$ converges.)
We can then have $x^* \approx \frac{1}{1-L}\left[\varphi\left (x_k\right)-L x_k\right]=\phi(x)$ which is a better approximation
([pdf](zotero://open-pdf/library/items/X3UESHXG?page=51&annotation=AEKYVJ4I))
The order of convergence of this method is $2$ if $L = \varphi^{'}(x^*)$ 
proof: 
$\phi^{'}(x)=\frac{1}{1-L}(\varphi^{'}(x^{*})-L)$ and if $L = \varphi^{'}(x^{*})$ then it converges locally with order $2$  ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=52&annotation=FLA4YZL8))
### [[Aitken's method]]


# programming implementation 
```matlab 
x = [x0]
varphix = inline('. ')
k=1
epsilon =  % set the stopping criterion 
while 1:
	xp1 = varphix(x(k))
	x = [x xp1]
	if abs(xp1-x(k)) < epsilon
		break 
	end
	k = k+1
end 
```