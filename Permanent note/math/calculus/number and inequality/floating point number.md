Floating point numbers are **[[scalar]] that do require decimal points**. Generally, floating point numbers can be expressed as {{
$f = \pm \omega \times \beta^J$     where $L \leq J \leq U$. 
$\beta$  is the base (二进制 $\beta = 2$, 十进制 $\beta = 10$ 以此类推), $J$ is the order and $\omega$ is the fraction.  <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F2AVWIQEV%22%2C%22annotationKey%22%3A%22C2TDWXMK%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2226%22%2C%22position%22%3A%7B%22pageIndex%22%3A25%2C%22rects%22%3A%5B%5B424.516%2C679.234%2C569.482%2C688.141%5D%2C%5B42.52%2C667.278%2C173.777%2C677.774%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F8EBIR37H%22%5D%2C%22locator%22%3A%2226%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/2AVWIQEV?page=26&#x26;annotation=C2TDWXMK">“floating point number”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F8EBIR37H%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/8EBIR37H">Grizzle</a></span>)</span>  ([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=28&annotation=VPVWRE9P)) }}
# Fraction  
For fractions, they have the form of $\omega = (0.d_1d_{2} \ldots d_t)_{\beta} = (\frac{d_1}{\beta^{1 }}+\frac{d_{2}}{\beta^{2}}+ \ldots + \frac{d_{t}}{\beta^t})$.  $d_{1}\neq 0$ and $0 \leq d_{i}< \beta$  
We call $t$ the length of $\omega$.  <!--SR:!2023-03-13,1,230-->

# Space between floating numbers 
It is defined as the difference between the nearby numbers in the fraction. 
For instance: If $x = 0. d_1d_{2} \times  10^{-1}$, then the space between each fraction is $0.01 \times 10^{-1}$ . 

Generally the calculation equation for space between floating numbers in interval $[\beta^{\alpha-1},\beta^{\alpha}]$ is :: $\beta^{\alpha-t}$.    <!--SR:!2023-03-15,3,250-->
([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=30&annotation=UJSF5DHR))
# Number of floating point numbers 
?
$n = 2 (\beta -1)\beta^{t-1}(U-L+1)+1$ where these numbers are symmetrically distributed in the interval $[m,M]$ and $[-M,m]$.  $m = \beta^{L-1}$ and $M = \beta^U(1-\beta^{-t})$ 
([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=36&annotation=BRZ7CL44))
## proof 
We can see that because $d_{1}\neq 0$, there is $\beta-1$ choices for it and $\beta$ choices for other digits. Therefore we have $(\beta-1)\beta^{t-1}$ for all the choices of digits. Because of the negative and positive situations, we need to times $2$. Considering exponents, $U-L+1$ exponents can be chosen. Finally, we should take $0$ into consideration and add $1$. The result is $2 (\beta-1)\beta^{t-1}(U-L+1)+1$  
## plotting floating point numbers 
we can plot these numbers using [[Matlab]] and the code is listed below: 
```matlab
clc;
clear; 
x=[] % create an empty vector 
for i=m:B^(-t):M
    for j=L:U
        x=[x, i*B^j]; 
    end
end
x=[x -x 0 ]
y=zeros(1,length(x)); 
plot(x,y,'r+')
```
<!--SR:!2023-03-15,3,250-->

# errors 
[[relative error - floating point number]]






