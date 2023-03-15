---
aliases: [convergence rate]
---
Suppose the sequence ${x_k}$ converges to $x^{*}$. The order of convergence is denoted as $p \geq 1$ and it is defined if :: $\frac{e_{k+1}}{e_{k}^{p}} \to c \neq 0$ as $k \to \infty$ where $e_{k}=x_{k}-x^{*}$ which is the [[absolute error]]. ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=39&annotation=32567C4E)) <!--SR:!2023-03-09,3,252-->
# [[convergent]] rate 
If $p$ is larger then the sequence converges faster. 
Proof: $\frac{e_{k+1}}{e_{k}} \to c$ means that $e_{k+1}=ce_{k}^{p}$  with $p$ becomes larger, $ce_{k}^{p}$ becomes smaller and $e_{k+1}$ becomes smaller.  ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=39&annotation=AY4W3HPP))

1. If $p=1$, we have $0 < |c|<1$ and the sequence is said to converge **linearly** 
2. If $p=2$, the sequence is said to converge **quadratically**
3. if $p>1$, then we said that it converges superlinearly.  <!--SR:!2023-03-10,4,270-->