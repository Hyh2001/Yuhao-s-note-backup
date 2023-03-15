Geometric series is the sum of [[geometric sequence]]. 
It is in the form of $\sum_{n\to \infty}s_{n}$ where $s_{n} = \sum_{n=0}^{\infty}x^{n}$

1. If $|x| < 1$, the sequence of partial sums $s_n = 1 + x +x^2+x^3+…+x^n$ is [[convergent]]  and it converges to $lim_{n \to \infty}s_n = \frac{1}{1-x}$
2. if $|x| \geq 1$, the series is [[divergent]] 

# Proof 
By algebra, we see that $s_n(1-x)=\left(1+x+x^2+x^3+\cdots+x^n\right)(1-x)=$  $1-x^{n+1}$. Therefore,

$s_n=\frac{1-x^{n+1}}{1-x}, \quad(x \neq 1)$

for $|x|<1$ we have $\lim _{n \rightarrow \infty} x^n=0$ and

$\lim _{n \rightarrow \infty} s_n=\lim _{n \rightarrow \infty}\left(1+x+x^2+x^3+\cdots+x^n\right)=\lim _{n \rightarrow \infty} \frac{1-x^{n+1}}{1-x}=\frac{1}{1-x}$

If $|x| \geq 1$, then $x^n$ does not approach zero, the series diverges.




1.  <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FYL3VT4CZ%22%2C%22annotationKey%22%3A%229BIHB675%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2229%22%2C%22position%22%3A%7B%22pageIndex%22%3A41%2C%22rects%22%3A%5B%5B126.753%2C516.059%2C197.966%2C526.022%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%2C%22locator%22%3A%2229%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/YL3VT4CZ?page=42&#x26;annotation=9BIHB675">“Geometric series”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%2C%22itemData%22%3A%7B%22id%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%2C%22type%22%3A%22book%22%2C%22collection-title%22%3A%22Undergraduate%20Texts%20in%20Mathematics%22%2C%22event-place%22%3A%22New%20York%2C%20NY%22%2C%22ISBN%22%3A%22978-1-4614-7945-1%22%2C%22language%22%3A%22en%22%2C%22note%22%3A%22DOI%3A%2010.1007%2F978-1-4614-7946-8%22%2C%22publisher%22%3A%22Springer%20New%20York%22%2C%22publisher-place%22%3A%22New%20York%2C%20NY%22%2C%22source%22%3A%22DOI.org%20(Crossref)%22%2C%22title%22%3A%22Calculus%20With%20Applications%22%2C%22URL%22%3A%22http%3A%2F%2Flink.springer.com%2F10.1007%2F978-1-4614-7946-8%22%2C%22author%22%3A%5B%7B%22family%22%3A%22Lax%22%2C%22given%22%3A%22Peter%20D.%22%7D%2C%7B%22family%22%3A%22Terrell%22%2C%22given%22%3A%22Maria%20Shea%22%7D%5D%2C%22accessed%22%3A%7B%22date-parts%22%3A%5B%5B%222022%22%2C12%2C19%5D%5D%7D%2C%22issued%22%3A%7B%22date-parts%22%3A%5B%5B%222014%22%5D%5D%7D%7D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/T6IUTL24">Lax 和 Terrell, 2014</a></span>)</span>