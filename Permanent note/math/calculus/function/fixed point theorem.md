---
aliases: [FPT]
---
Suppose that a function $\varphi(x)$ is [[continuity|continuous]] on $[a,b]$, and $\varphi (x) \in [a,b]$ for all $x \in [a, b]$. Then $\exists \xi \in [a,b]$ such that $\xi = \varphi(\xi)$ ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=6&annotation=MTSCEIWG))
There are infinite choices of the function $\varphi$ and it is important to find a $\varphi$ that satisfies the assumption above. ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=7&annotation=WI93DAVY))
# proof 
We can let $f (x) = x - \varphi(x)$. Then it is obvious that $f (a) = a - \varphi (a) \leq 0$ and $f (b) = b -\varphi (b) \geq 0$ thus $f (a) f (b) \leq 0$. With the definition of $\varphi(x)$, $f (x)$ is also continuous on the closed interval $[a,b]$. Therefore, by the [[intermediate value theorem]], we can find a $n \in [a,b]$ such that $f (n) = 0$. ([Ascher 和 Greif, 2011, p. 63](zotero://select/library/items/HJK4ZQRP)) ([pdf](zotero://open-pdf/library/items/FSDKG9DD?page=63&annotation=BEUIMM3J))
Moreover, we want to know when the uniqueness of root. We can see [[fixed point iteration - global convergence#^a4dc62]] for the proof of uniqueness of root. 