We denote central difference approximation as :: $f^{'}(x) = \frac{f(x + h) - f(x-h)}{2h}$ where $h$ is sufficiently close to $0$ for real numbers. However, for computer applications, $h$ should be properly chosen.  ([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=22&annotation=PJPQVIZF)) <!--SR:!2023-03-08,2,230-->

# Derivation 
Using the definition of [[derivative]], we can have that $f^{'}(x) = lim_{\delta x \to 0}\frac{f(x + \delta x) - f(x)}{\delta x}$. We can consider both the case where $\delta x =h$ or $\delta x = -h$ for $h = 0$. We will have two approximations that $f^{'}(x) \simeq \frac{f(x+h)-f(x)}{h}$ or $f^{'}(x) \simeq \frac{f(x)-f(x-h)}{h}$. By equating both sides we can have $f^{'}(x) = \frac{f(x + h) - f(x-h)}{2h}$. 
([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=22&annotation=KDEAUPRD))

# disadvantage 
If $h$ is too small then we may get into a condition where :: $f (x+h) - f (x-h) = 0$. To solve this problem we can change the formula to avoid using minus.  <!--SR:!2023-03-08,3,250-->
## example 
$f^{' (2)} \simeq \frac{\sqrt{2+h}-\sqrt{2-h}}{2h}$, we can change it to :: $\frac{1}{\sqrt{2+h}+\sqrt{2-h}}$ <!--SR:!2023-03-08,2,230-->
([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=56&annotation=GFHA9RCS))

   