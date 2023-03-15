---
aliases: [geometric progression]
---
Sequences of numbers that follow the pattern of multiplying by a fixed number to get the next term are called geometric sequence.  It is denoted by $\left\{r^n\right\}$

# properties

(a) converges if $|r|<1$ , and in this case, $\lim _{n \rightarrow \infty} r^n=0$ ,

(b) converges if $r=1$ , and in this case, $\lim _{n \rightarrow \infty} 1^n=1$ ,

(c) diverges for $r>1$  and for $r \leq-1$ .

## proof  

(a) If $0 \leq r<1$, then $\left\{r^n\right\}$ is a decreasing sequence that is bounded, $\left|r^n\right| \leq 1$. Therefore, by the monotone convergence theorem it converges to a limit \$a\$. The sequence $r, r^2, r^3, \ldots$ has the same limit as $1, r, r^2, r^3, \ldots$, and so by Theorem 1.6,

$a=\lim _{n \rightarrow \infty} r^{n+1}=\lim _{n \rightarrow \infty} r r^n=r \lim _{n \rightarrow \infty} r^n=r a$

and $a(r-1)=0$. Now since $r \neq 1, a=0$.

If $-1<r<0$, then each power $r^n$ has the same distance to 0 as $|r|^n$, so again the limit is 0 .

(b) For any tolerance $\varepsilon,\left|1^n-1\right|=0<\varepsilon$ , so the limit is clearly 1 .

(c) To show that $\left\{r^n\right\}$ diverges for \$|r|>1\$ or $r=-1$, suppose the limit exists: $\lim _{n \rightarrow \infty} r^n=a$ . By the argument in part (a), the limit must be 0 . But this is not possible. We know that $\left|r^n-0\right| \geq 1$ for all $n$, i.e., the distance between $r^n$ and 0 is always at least 1 , so $r^n$ does not tend to 0 .




1. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FYL3VT4CZ%22%2C%22annotationKey%22%3A%22U2SGFCJY%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2227%22%2C%22position%22%3A%7B%22pageIndex%22%3A39%2C%22rects%22%3A%5B%5B125.281%2C564.148%2C376.624%2C573.274%5D%2C%5B62.88%2C552.268%2C376.771%2C561.394%5D%2C%5B62.88%2C540.268%2C116.071%2C549.394%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%2C%22locator%22%3A%2227%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/YL3VT4CZ?page=40&#x26;annotation=U2SGFCJY">“geometric sequence”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%2C%22itemData%22%3A%7B%22id%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%2C%22type%22%3A%22book%22%2C%22collection-title%22%3A%22Undergraduate%20Texts%20in%20Mathematics%22%2C%22event-place%22%3A%22New%20York%2C%20NY%22%2C%22ISBN%22%3A%22978-1-4614-7945-1%22%2C%22language%22%3A%22en%22%2C%22note%22%3A%22DOI%3A%2010.1007%2F978-1-4614-7946-8%22%2C%22publisher%22%3A%22Springer%20New%20York%22%2C%22publisher-place%22%3A%22New%20York%2C%20NY%22%2C%22source%22%3A%22DOI.org%20(Crossref)%22%2C%22title%22%3A%22Calculus%20With%20Applications%22%2C%22URL%22%3A%22http%3A%2F%2Flink.springer.com%2F10.1007%2F978-1-4614-7946-8%22%2C%22author%22%3A%5B%7B%22family%22%3A%22Lax%22%2C%22given%22%3A%22Peter%20D.%22%7D%2C%7B%22family%22%3A%22Terrell%22%2C%22given%22%3A%22Maria%20Shea%22%7D%5D%2C%22accessed%22%3A%7B%22date-parts%22%3A%5B%5B%222022%22%2C12%2C19%5D%5D%7D%2C%22issued%22%3A%7B%22date-parts%22%3A%5B%5B%222014%22%5D%5D%7D%7D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/T6IUTL24">Lax 和 Terrell, 2014</a></span>)</span>