This method is used to solve an [[upper-triangular matrix]] system. This method first solves $x_n$ and then use $x_n$ to solve for $x_{n-1}$ and iteratively to finally find $x_1$.
# Julia implementation

```julia 
function backwardsub(U, b)   
# U a square upper triangular matrix   
# b has same number of rows as U   
# assert that no entries on the diagonal of U are 0 or very close to 0   
	if minimum(abs.(diag(U))) < 1e-6     
		return false   
	end   
	n = length(b)   
	x = Vector{Float64}(undef,n)   
# we start from the bottom and work our way to the top   
	x[n] = b[n]/U[n,n]   
	for i = n-1 : -1:1     
	#x[i] = (b[i] - U[i,(i+1):n]' * x[(i+1):n]) / U[i,i]   
			x[i] = (b[i] - (U[i,(i+1):n] * x[(i+1):n])[1]) / U[i,i]   
	end  
	return x  
end  
```









1. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F2AVWIQEV%22%2C%22annotationKey%22%3A%22MZTYZRUU%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2247%22%2C%22position%22%3A%7B%22pageIndex%22%3A46%2C%22rects%22%3A%5B%5B114.05%2C713.4%2C553.892%2C722.426%5D%2C%5B58.11%2C701.445%2C161.353%2C710.471%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F8EBIR37H%22%5D%2C%22locator%22%3A%2247%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/2AVWIQEV?page=47&#x26;annotation=MZTYZRUU">“back substitution”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F8EBIR37H%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/8EBIR37H">Grizzle</a></span>)</span>
