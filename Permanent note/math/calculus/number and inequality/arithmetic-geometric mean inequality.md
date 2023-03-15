---
aliases: [A-G inequality]
---
#calculus #review 
# for two numbers
It is in the form of $\sqrt{ab} \leq \frac{a+b}{2}$, with equality only in $a = b$. It can be used to show that among all the rectangles have the same perimeter, square has the largest area. 
## proof
$(a+b)^2 - 4ab = a^2 +b^2-2ab = (a-b)^2 \geq 0$ 

# for n numbers 
$(a_1a_2…a_n)^{1/n} \leq \frac{a_1 + a_2 +.. +a_n}{n}$ with equality holding when $a_1 =a_2 =.. = a_n$
## proof 
We use mathematical inductions. 
let $a = \frac{c +d}{2}$, $b = \frac{e + f}{2}$, then with $\sqrt{ab} \leq \frac{a+b}{2}$ we can proof $\sqrt{cdef} \leq ab$ and thus $(cdef)^{\frac{1}{4}} \leq \frac{c+d+e+f}{4}$ therefore we proof the theorem for even numbers.
let $m = \frac{a+b+c}{3}$, then $m = \frac{a+b+c+m}{4}$, therefore, we can have that $m \geq (abcm)^{\frac{1}{4}}$ and we get $m \geq (abc)^{\frac{1}{3}}$ we proof this for odd numbers.

# applications
1. to approach some numbers: Let $r$ be a real number and if we want to approach it, we can define a series as $s_n = \frac{1}{2}(s_{n-1}+\frac{r^2}{s_{n-1}})$  and use A-G inequality we can find that $\frac{1}{2}(s_{n-1}+\frac{r^2}{s_{n-1}}) \geq r$ and get $=$ when $s_{n-1} = \sqrt{r}$.  Therefore, $s_n$ will gradually approach to $\sqrt{r}$. 


1. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FYL3VT4CZ%22%2C%22annotationKey%22%3A%22LPXH6G8C%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%225%22%2C%22position%22%3A%7B%22pageIndex%22%3A17%2C%22rects%22%3A%5B%5B317.162%2C442.588%2C376.711%2C451.594%5D%2C%5B62.88%2C430.588%2C320.777%2C439.594%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%2C%22locator%22%3A%225%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/YL3VT4CZ?page=18&#x26;annotation=LPXH6G8C">“The geometric mean of two positive numbers is less than their arithmetic mean:”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/T6IUTL24">Lax 和 Terrell, 2014</a></span>)</span>
2. 