#calculus/limit #review #calculus/series 

1. If $f(x) \leq g(x)$ when $x$ is near $a$ (except possibly at $a$) and the limits of $f$ and $g$ both exist as $x$ approaches $a$, then
   $lim_{x \to a}f(x) \leq lim_{x \to a}g(x)$
2. If $f(x) \leq g(x) \leq h(x)$ when $x$ is near $a$ (except possibly at $a$) and
   $lim_{x \to a}f(x) = lim_{x \to a}h(x) = L$
   then, $lim_{x \to a}g(x) = L$
([Lax 和 Terrell, 2014, p. 62](zotero://select/library/items/T6IUTL24)) ([pdf](zotero://open-pdf/library/items/YL3VT4CZ?page=74&annotation=FKTS65YD))
## proof 


## squeeze for [[sequence]]s 
Suppose that for all $n>N$ ,

$a_n \leq b_n \leq c_n$

and that $\lim _{n \rightarrow \infty} a_n=\lim _{n \rightarrow \infty} c_n=a$ . Then $\lim _{n \rightarrow \infty} b_n=a$ .

## Proof
Subtracting $a$ from the inequalities, we get

$a_n-a \leq b_n-a \leq c_n-a$

Let $\varepsilon>0$  be any [[tolerance]]. Since $\left\{a_n\right\}$  and $\left\{c_n\right\}$ have [[limit]] $a$, there is a number $N_1$ such that when $n>N_1, a_n$ is within $\varepsilon$ of $a$, and there is a number $N_2$ such that when $n>N_2, c_n$ is within $\varepsilon$ of $a$. Let $M$ be the largest of $N, N_1$, and $N_2$. Then when $n>M$, we get

$-\epsilon<a_n-a \leq b_n-a \leq c_n-a<\epsilon$

So for the middle term, we see that $\left|b_n-a\right|<\varepsilon$  This shows that $b_n$ converges to $a$






1. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FYL3VT4CZ%22%2C%22annotationKey%22%3A%2268MDL5NJ%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2222%22%2C%22position%22%3A%7B%22pageIndex%22%3A34%2C%22rects%22%3A%5B%5B121.685%2C405.779%2C211.385%2C415.742%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%2C%22locator%22%3A%2222%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/YL3VT4CZ?page=35&#x26;annotation=68MDL5NJ">“The squeeze theorem”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/T6IUTL24">Lax 和 Terrell, 2014</a></span>)</span>