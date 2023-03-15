Given two numbers $a,b$ where $a>b$ we can calculate their arithmetic mean as $a_1 = \frac{a+b}{2}$ and geometric mean as $g_1 = \sqrt{ab}$. We can have the relationship that $b \leq g_1 \leq a_1 \leq a$ based on [[arithmetic-geometric mean inequality]] . Repeat the process with new arithmetic mean and geometric mean, we get several [[nested interval]]  $[g_n,a_n]$.  

The interval between the arithmetic and geometric means of $a$ and $g$ is less than or equal to half the length of the interval between $a$ and $g$ which means that $a_{1}- g_{1}\leq \frac{1}{2}(a-g)$.

And finally the process squeezes in on exactly one number which is called the arithmetic-geometric mean of $a$ and $g$. $AGM(a,g) = lim_{n \to \infty} a_n = \lim_{n \to \infty}g_n$





1. “AGM” ([Lax 和 Terrell, 2014, p. 36](zotero://select/library/items/T6IUTL24)) ([pdf](zotero://open-pdf/library/items/YL3VT4CZ?page=49&annotation=7HCRSAH3))