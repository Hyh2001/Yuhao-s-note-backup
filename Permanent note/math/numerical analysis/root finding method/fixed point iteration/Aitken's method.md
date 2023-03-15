We can use :: $x_{k+1}=\varphi\left(\varphi\left(x_k\right)\right)-\frac{\left(\varphi\left(\varphi\left(x_k\right)\right)-\varphi\left(x_k\right)\right)^2}{\varphi\left(\varphi\left(x_k\right)\right)-2 \varphi\left(x_k\right)+x_k}$ to replace the original $\varphi(x)$ ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=55&annotation=JSTLH68U)) <!--SR:!2023-03-09,3,250-->
# proof 
We know that $\lim_{k\to \infty} =\frac{x_{k+1}-x^{*}}{x_{k}-x^{*}} = \varphi^{'}(x^{*})$ when $k$ is large, this [[limit]] is true for both $x_{k+1}$ and $x_{k+2}$. We can have the relationship 
$\frac{x_{k+2}-x^*}{x_{k+1}-x^*} \approx\varphi^{\prime}\left (x^*\right) \approx \frac{x_{k+1}-x^*}{x_k-x^*}$
which implies
$$
\begin{aligned}
x^* & \approx x_{k+2}-\frac{\left(x_{k+2}-x_{k+1}\right)^2}{x_{k+2}-2 x_{k+1}+x_k} \quad x_{\varphi_{+2}}=\varphi\left(\underline{\underline{x_{h+1}}}\right) \\
& =\varphi\left(\varphi\left(x_k\right)\right)-\frac{\left(\varphi\left(\varphi\left(x_k\right)\right)-\varphi\left(x_k\right)\right)^2}{\varphi\left(\varphi\left(x_k\right)\right)-2 \varphi\left(x_k\right)+x_k} .
\end{aligned}$$

([pdf](zotero://open-pdf/library/items/X3UESHXG?page=56&annotation=3QBFRK9T))
# merit of this method 
1. $\varphi^{\prime}(x)$ is **not involved** 
2. This method converges **locally with order $2$** ([pdf](zotero://open-pdf/library/items/X3UESHXG?page=57&annotation=7FPIQ9UV))