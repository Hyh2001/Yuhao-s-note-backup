#calculus/series 
Series is the sum of terms of a :: [[sequence]]. We can build a series by adding the numbers of a sequence: $s_n = \sum_{j=1}^na_j$. 

If $lim_{n \to \infty}s_n$ exists, then the series $\sum_{n=1}^{\infty}a_n$ :: converges. Otherwise it diverges. $a_n$ is called the terms of the series.

If $\sum_{n=1}^{\infty}a_n$ converges, then :: $\lim_{n \to \infty}a_n = 0$

Proof: 
? 
Let $s_n=a_1+\cdots+a_n$ . Since $\sum_{n=1}^{\infty} a_n$  converges, the limit $\lim _{n \rightarrow \infty} s_n=L$  exists, and for the shifted sequence $\lim _{n \rightarrow \infty} s_{n-1}=L$  as well. According to Theorem 1.6,

$\lim _{n \rightarrow \infty} a_n=\lim _{n \rightarrow \infty}\left(s_n-s_{n-1}\right)=L-L=0$













1. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FYL3VT4CZ%22%2C%22annotationKey%22%3A%22VVSM3U7E%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2220%22%2C%22position%22%3A%7B%22pageIndex%22%3A32%2C%22rects%22%3A%5B%5B302.52%2C126.988%2C385.545%2C136.114%5D%2C%5B53.879%2C114.988%2C279.862%2C124.114%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%2C%22locator%22%3A%2220%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/YL3VT4CZ?page=33&#x26;annotation=VVSM3U7E">“series"</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%2C%22itemData%22%3A%7B%22id%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%2C%22type%22%3A%22book%22%2C%22collection-title%22%3A%22Undergraduate%20Texts%20in%20Mathematics%22%2C%22event-place%22%3A%22New%20York%2C%20NY%22%2C%22ISBN%22%3A%22978-1-4614-7945-1%22%2C%22language%22%3A%22en%22%2C%22note%22%3A%22DOI%3A%2010.1007%2F978-1-4614-7946-8%22%2C%22publisher%22%3A%22Springer%20New%20York%22%2C%22publisher-place%22%3A%22New%20York%2C%20NY%22%2C%22source%22%3A%22DOI.org%20(Crossref)%22%2C%22title%22%3A%22Calculus%20With%20Applications%22%2C%22URL%22%3A%22http%3A%2F%2Flink.springer.com%2F10.1007%2F978-1-4614-7946-8%22%2C%22author%22%3A%5B%7B%22family%22%3A%22Lax%22%2C%22given%22%3A%22Peter%20D.%22%7D%2C%7B%22family%22%3A%22Terrell%22%2C%22given%22%3A%22Maria%20Shea%22%7D%5D%2C%22accessed%22%3A%7B%22date-parts%22%3A%5B%5B%222022%22%2C12%2C19%5D%5D%7D%2C%22issued%22%3A%7B%22date-parts%22%3A%5B%5B%222014%22%5D%5D%7D%7D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/T6IUTL24">Lax 和 Terrell, 2014</a></span>)</span>
2. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FYL3VT4CZ%22%2C%22annotationKey%22%3A%22DJ5D25V8%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2228%22%2C%22position%22%3A%7B%22pageIndex%22%3A40%2C%22rects%22%3A%5B%5B153.601%2C385.468%2C254.158%2C394.594%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%2C%22locator%22%3A%2228%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/YL3VT4CZ?page=41&#x26;annotation=DJ5D25V8">“partial sums of the series”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%5D%2C%22itemData%22%3A%7B%22id%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FT6IUTL24%22%2C%22type%22%3A%22book%22%2C%22collection-title%22%3A%22Undergraduate%20Texts%20in%20Mathematics%22%2C%22event-place%22%3A%22New%20York%2C%20NY%22%2C%22ISBN%22%3A%22978-1-4614-7945-1%22%2C%22language%22%3A%22en%22%2C%22note%22%3A%22DOI%3A%2010.1007%2F978-1-4614-7946-8%22%2C%22publisher%22%3A%22Springer%20New%20York%22%2C%22publisher-place%22%3A%22New%20York%2C%20NY%22%2C%22source%22%3A%22DOI.org%20(Crossref)%22%2C%22title%22%3A%22Calculus%20With%20Applications%22%2C%22URL%22%3A%22http%3A%2F%2Flink.springer.com%2F10.1007%2F978-1-4614-7946-8%22%2C%22author%22%3A%5B%7B%22family%22%3A%22Lax%22%2C%22given%22%3A%22Peter%20D.%22%7D%2C%7B%22family%22%3A%22Terrell%22%2C%22given%22%3A%22Maria%20Shea%22%7D%5D%2C%22accessed%22%3A%7B%22date-parts%22%3A%5B%5B%222022%22%2C12%2C19%5D%5D%7D%2C%22issued%22%3A%7B%22date-parts%22%3A%5B%5B%222014%22%5D%5D%7D%7D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/T6IUTL24">Lax 和 Terrell, 2014</a></span>)</span>