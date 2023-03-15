For [[floating point number]] s, their [[relative error]] s are [[bounded]] and we use $\eta$ to denote it (This $\eta$ is called **[[machine precision]]**). ([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=43&annotation=S9NSNC7S))
$|E_{r}| = |\frac{fl (x)-x}{x}| \leq \eta$ 

With the approximations, we can have two theorems: 
## theorem 1 
Suppose that $x = \pm 0. a_1a_{2}\ldots a_{l} \times 10^m$ is an approximation to $x^{*}$ and $x$ has $n$ [[significant digit]]. Then 
::  $|E_{r}| = |\frac{x-x^{*}}{x}| \leq \frac{1}{2a_{1}}\times 10^{-n+1}$ 
### proof 
We can see that $x$ has $n$ significant digits means $|x-x^{*}| \leq \frac{1}{2} \times 10^{m-n}$. 
for  $|x| > 0. a_{1} \times 10^{m}$ (this can be proved based on the definition of $x$) ,  $|E_{r}|\leq \frac{\frac{1}{2} \times 10^{m-n}}{a_{1}\times 10^{m-1}} = \frac{1}{2a_{1}}\times 10^{-n+1}$ ([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=50&annotation=CE9UZ89T))
## theorem 2 
Suppose that $x = \pm 0. a_1a_{2}\ldots a_{l} \times 10^{m}$  is an approximation to $x^{*}$ and $x$ then it has the [[relative error bound]], ::  $|E_{r}| = |\frac{x-x^{*}}{x}| \leq \frac{1}{2a_{1}+1}\times 10^{-n+1}$ and $x$ has $n$ significant digit
### proof 
for $|x| \leq (0.a_{1}+0.1) \times 10^{m}$ (this can be proved based on the definition of $x$), we can have: $|x -x^{*}| = |\frac{x - x^{*}}{x}| \cdot |x| \leq \frac{1}{2 (a_{1}+1)}\times 10^{-n+1} \times (a_{1}+1)\times 10^{m-1} = \frac{1}{2} \times 10^{m-n}$
([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=51&annotation=3SNPRWQ9))
 