# existence of root
The [[fixed point theorem]] has guaranteed that the function $\varphi(x)$ will have a solution if it follows the restriction. 
# [[convergent]] of the iterative [[sequence]] $x_k$
If the iterative sequence is convergent and it approaches to a limit we call it $x^*$. We can proof that $x^*$ is a root to $\varphi (x) = x$ or it is a fixed point to $\varphi(x)$. 
Proof: $x^{*}= \lim_{k \to \infty} x_{k+1} = lim_{k\to \infty}\varphi (x_{k})= \varphi (\lim_{k \to \infty} x_{k})= \varphi(x^*)$ 
([pdf](zotero://open-pdf/library/items/X3UESHXG?page=13&annotation=D3BVPD4H))
## proof of the convergence 
Suppose that $x^*$ is a root to $x = \varphi(x)$. Then we can use [[mean value theorem]], to proof that $x^{*}- x_{k+1} = \varphi (x^{*})-\varphi (x_{k})= \varphi^{'}(\xi)(x^{*}-x_k)$ (The first equivalent uses the definition of fixed point). 
Then we can easily see that if 
$\exists 0 <L<1$  such that $|\varphi^{'}(x)| \leq L, \forall x \in [a,b]$ and $x_{k}\in [a,b]$. We have: 
$|x^{*} - x_{k+1}|\leq L|x^{*}-x_{k}|$
and inductively, we get 
$|e_{k}| \leq L^{k}|e_{0}| \to 0$, as $k \to \infty$ where $e_{k}=x_{k}- x^{*}$ 
([pdf](zotero://open-pdf/library/items/X3UESHXG?page=18&annotation=BNGJVWL2))  ([Ascher 和 Greif, 2011, p. 64](zotero://select/library/items/HJK4ZQRP)) ([pdf](zotero://open-pdf/library/items/FSDKG9DD?page=64&annotation=QQ53M8AG))

# error of the iterative method 
The two equations will hold: 
1. $|x^{*}-x_{k}|\leq \frac{1}{1-L}|x_{k+1}-x_{k}|$
2. $|x^{*}-x_{k}|\leq \frac{L^{k}}{1-L}|x_{1}-x_{0}|$ 
([pdf](zotero://open-pdf/library/items/X3UESHXG?page=21&annotation=HIGJKAU3))

## proof of uniqueness 

We assume there are two roots $x^*$ and $\bar{x^*}$. Because they are two roots, we will have the formula: 
$|x^{*}-\bar{x^{*}}| =|\varphi (x^{*)}-\varphi (\bar{x^{*})|}\leq L|x^{*}-\bar{x^*}|$ from both sides we can get: 
$(1-L)|x^{*}-\bar{x^{*}}| \leq 0$ but actually $1-L > 0$ so there can not exist two roots. 
([pdf](zotero://open-pdf/library/items/X3UESHXG?page=22&annotation=47WMPY2M))  ([Ascher 和 Greif, 2011, p. 64](zotero://select/library/items/HJK4ZQRP)) ([pdf](zotero://open-pdf/library/items/FSDKG9DD?page=64&annotation=CSHB2PCU))

## proof of error 
1. We can see that $(1-L)|x^{*} -x_{k}|= |x^{*}-x_{k}| - L|x^{*}-x_{k}| \leq |x^{*}-x_{k}| - |x^{*}-x_{k+1}| \leq |x_{k+1}-x_{k}|$
	1. The first inequality can be proved by $|x^{*} - x_{k+1}| = |\varphi (x^{*}) -\varphi (x_{k})| = |\varphi^{'}(\xi)(x^{*}-x_{k)}|\leq L|(x^{*}-x_k)|$ 
	2. The second inequality can be proved by using the number line 
			1. If $x_k$ and $x_{k+1}$ are on the same side $|x^{*}-x_{k}| - |x^{*}-x_{k+1}| = |x_{k+1}-x_{k}|$
			2. If $x_k$ and $x_{k+1}$ are on the different side $|x^{*}-x_{k}| - |x^{*}-x_{k+1}| < |x_{k+1}-x_{k}|$
Thus the error 1 is proved ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=24&annotation=T2SZ67JQ))
2. Because $|x_{k+1} -x_{k}| \leq L|x_{k}-x_{k-1}|$ then we can recursive apply the equation to $|x^{*}-x_{k}|\leq \frac{1}{1-L}|x_{k+1}-x_{k}|$ and we will proof the error 2 ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=24&annotation=ZJGE6D98))