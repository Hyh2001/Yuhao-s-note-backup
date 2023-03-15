#calculus

Euler's number is denoted as $e$ and it is defined as the number such that $\frac{de^x}{dx} = e^x$. Its [[sequence]] form is $e = lim_{n \to \infty}(1+\frac{1}{n})^n$
 <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FYL3VT4CZ%22%2C%22annotationKey%22%3A%22SLCKDYMX%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2244%22%2C%22position%22%3A%7B%22pageIndex%22%3A56%2C%22rects%22%3A%5B%5B175.575%2C356.788%2C239.943%2C365.914%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%2C%22locator%22%3A%2244%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/YL3VT4CZ?page=57&#x26;annotation=SLCKDYMX">“Euler’s number”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%2C%22itemData%22%3A%7B%22id%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%2C%22type%22%3A%22book%22%2C%22collection-title%22%3A%22Undergraduate%20Texts%20in%20Mathematics%22%2C%22event-place%22%3A%22New%20York%2C%20NY%22%2C%22ISBN%22%3A%22978-1-4614-7945-1%22%2C%22language%22%3A%22en%22%2C%22note%22%3A%22DOI%3A%2010.1007%2F978-1-4614-7946-8%22%2C%22publisher%22%3A%22Springer%20New%20York%22%2C%22publisher-place%22%3A%22New%20York%2C%20NY%22%2C%22source%22%3A%22DOI.org%20(Crossref)%22%2C%22title%22%3A%22Calculus%20With%20Applications%22%2C%22URL%22%3A%22http%3A%2F%2Flink.springer.com%2F10.1007%2F978-1-4614-7946-8%22%2C%22author%22%3A%5B%7B%22family%22%3A%22Lax%22%2C%22given%22%3A%22Peter%20D.%22%7D%2C%7B%22family%22%3A%22Terrell%22%2C%22given%22%3A%22Maria%20Shea%22%7D%5D%2C%22accessed%22%3A%7B%22date-parts%22%3A%5B%5B%222022%22%2C12%2C19%5D%5D%7D%2C%22issued%22%3A%7B%22date-parts%22%3A%5B%5B%222014%22%5D%5D%7D%7D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/T6IUTL24">Lax 和 Terrell, 2014</a></span>)</span>
We want to investigate on the [[monotone]] and [[bounded]] of this sequence 
## monotonicity 
By using A-G inequality we can see that:

$\left(a_1 a_2 \cdots a_{n+1}\right)^{1 /(n+1)} \leq \frac{1}{n+1}\left(a_1+a_2+\cdots+a_{n+1}\right)$

Take the $n+1$ numbers as

$\underbrace{\left(1+\frac{1}{n}\right), \ldots,\left(1+\frac{1}{n}\right)}_{n \text { times }}, 1$

we can have that

$\left(1+\frac{1}{n}\right)^n<\left(1+\frac{1}{n+1}\right)^{n+1}$ which means that $e_{n+1} > e_n$ and the sequence is increasing
 ([Lax 和 Terrell, 2014, p. 45](zotero://select/library/items/T6IUTL24)) ([pdf](zotero://open-pdf/library/items/YL3VT4CZ?page=58&annotation=X3JF8CJH))
## boundedness 
We define $f_n = (1+\frac{1}{n})^{n+1}$ and we can find that this is a decreasing sequence by using $f_n = \frac{1}{(1-\frac{1}{n})^n}$ where $(1-\frac{1}{n})^n$ is an increasing sequence.

We know that $f_1=4\geq f_n >e_n$, So $e_n$ is bounded above while $f_n$ is bounded below by $0$.

Also we want to prove that $f_n$ and $e_n$ all converges to $e$. We first prove that they converge to a same number: $f_n - e_n = (1+\frac{1}{n})^{n+1} - (1+\frac{1}{n})^n=\frac{e_n}{n}$ with $n \to \infty$, this formula tends to $0$.

Both $f_n$ and $g_n$ converges slowly to $e$, we can use $g_n = 1 + 1+ \frac{1}{2!} + \frac{1}{3!} + … +\frac{1}{n!}$ which converges more quickly
 ([Lax 和 Terrell, 2014, p. 46](zotero://select/library/items/T6IUTL24)) ([pdf](zotero://open-pdf/library/items/YL3VT4CZ?page=59&annotation=EFBIAX8F))
# applications of this number 
1.  Financial motivation:
	1. Suppose you invest one dollar at the interest rate of $100\%$ per year. If the interest is compounded annually, a year later you will receive two dollars, that is, the original dollar invested plus another dollar for interest. If interest is compounded semiannually, you will receive at the end of the year $(1.5) \times 2 = 2.25$ dollars. That is $50\%$ interest after six months, giving you a value of $1.50$, followed by another six months during which you earn $50\%$ interest on your $1.50$. If interest is compounded n times a year, you will receive at the end of the year $(1+\frac{1}{n})^n$ dollars
 <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FYL3VT4CZ%22%2C%22pageLabel%22%3A%2244%22%2C%22position%22%3A%7B%22pageIndex%22%3A56%2C%22rects%22%3A%5B%5B190.967%2C204.028%2C385.655%2C213.154%5D%2C%5B53.88%2C192.028%2C385.559%2C201.154%5D%2C%5B53.88%2C180.148%2C385.481%2C189.274%5D%2C%5B53.88%2C168.148%2C385.584%2C177.274%5D%2C%5B53.88%2C155.819%2C385.735%2C167.183%5D%2C%5B53.88%2C144.268%2C385.642%2C153.393%5D%2C%5B53.88%2C131.939%2C385.58%2C141.902%5D%2C%5B53.879%2C114.388%2C85.653%2C123.514%5D%2C%5B87.959%2C128.099%2C95.291%2C138.062%5D%2C%5B95.278%2C114.059%2C117.059%2C130.233%5D%2C%5B112.08%2C107.668%2C117.061%2C116.674%5D%2C%5B118.2%2C126.559%2C129.206%2C138.062%5D%2C%5B132.12%2C114.388%2C161.877%2C123.514%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%2C%22locator%22%3A%2244%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/YL3VT4CZ?page=57">“financial applications”</a></span>    <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%2C%22itemData%22%3A%7B%22id%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%2C%22type%22%3A%22book%22%2C%22collection-title%22%3A%22Undergraduate%20Texts%20in%20Mathematics%22%2C%22event-place%22%3A%22New%20York%2C%20NY%22%2C%22ISBN%22%3A%22978-1-4614-7945-1%22%2C%22language%22%3A%22en%22%2C%22note%22%3A%22DOI%3A%2010.1007%2F978-1-4614-7946-8%22%2C%22publisher%22%3A%22Springer%20New%20York%22%2C%22publisher-place%22%3A%22New%20York%2C%20NY%22%2C%22source%22%3A%22DOI.org%20(Crossref)%22%2C%22title%22%3A%22Calculus%20With%20Applications%22%2C%22URL%22%3A%22http%3A%2F%2Flink.springer.com%2F10.1007%2F978-1-4614-7946-8%22%2C%22author%22%3A%5B%7B%22family%22%3A%22Lax%22%2C%22given%22%3A%22Peter%20D.%22%7D%2C%7B%22family%22%3A%22Terrell%22%2C%22given%22%3A%22Maria%20Shea%22%7D%5D%2C%22accessed%22%3A%7B%22date-parts%22%3A%5B%5B%222022%22%2C12%2C19%5D%5D%7D%2C%22issued%22%3A%7B%22date-parts%22%3A%5B%5B%222014%22%5D%5D%7D%7D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/T6IUTL24">Lax 和 Terrell, 2014</a></span>)</span>

[[Matlab Euler's number]]


 
