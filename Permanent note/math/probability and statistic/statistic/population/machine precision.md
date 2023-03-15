$\eta = \frac{1}{2}\beta^{1-t}$ by [[rounding]], 
$\eta = \beta^{1-t}$ by [[chopping]]
(the definition of $\beta$ and $t$ can be seen in card for [[floating point number]])
We can simplify the denotation into one equation: 
$fl (x) = x(1+\delta)$ where $|\delta|\leq \eta$ 
# proof 
we can proof the theorem as follow: 
we assume $x \neq 0$ and $x>0$. Let $\alpha$ be an integer such that: 
$\beta^{\alpha -1} \leq x < \beta^{\alpha}$. 
we can construct its floating point number representation as: 
$(0. d_1d_{2\ldots}d_t)_{\beta} \times \beta^{\alpha}$ 
they distributed in the interval with distance $\beta^{\alpha -t}$. 
Therefore, the biggest rounding error is: 
$|fl (x) - x| \leq \frac{1}{2}\beta^{\alpha -t} = \frac{1}{2}\beta^{\alpha-1}\beta^{1-t} \leq \frac{1}{2}x\beta^{1-t}$ 
and the relative error is $|E_{r}|\leq \frac{1}{2}\beta^{1-t}$ 
Same to the previous steps: the biggest chopping error is: 
$|E_{r}| \leq \beta^{1-t}$ 
([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=43&annotation=S9NSNC7S))