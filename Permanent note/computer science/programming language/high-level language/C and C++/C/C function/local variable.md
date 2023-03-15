函数中定义的变量称为局部变量（Local Variable），由于 [[C parameter|形参]] 相当于函数中定义的变量，所以形参也相当于局部变量。
# properties
1. 某个函数中定义的变量不能被另一个函数使用
2. 每次调用函数时局部变量都表示不同的存储空间。局部变量是在每次函数调用时分配存储空间，每次函数返回时释放存储空间的：存储空间不同导致每次调用这个函数时局部变量的初值可能不一样，运行环境不同，函数的调用次序不同，都会影响到局部变量的初值。
3. 局部变量可以用任意类型相符的表达式来初始化

# [[scope]] of local variable  
局部变量的作用域仅限于定义它的函数之中。



# [[global variable - local variable]] 




1. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F4IHU78F5%22%2C%22pageLabel%22%3A%2257%22%2C%22position%22%3A%7B%22pageIndex%22%3A56%2C%22rects%22%3A%5B%5B82%2C674.85%2C530.5%2C689.61%5D%2C%5B46%2C659.85%2C214%2C674.61%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22locator%22%3A%2257%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/4IHU78F5?page=57">“local variable”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/I2QD5IEX">“LinuxC”</a></span>)</span>
2. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F4IHU78F5%22%2C%22annotationKey%22%3A%22XJQVWKAN%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2257%22%2C%22position%22%3A%7B%22pageIndex%22%3A56%2C%22rects%22%3A%5B%5B64.744%2C632.85%2C304.744%2C647.61%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22locator%22%3A%2257%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/4IHU78F5?page=57&#x26;annotation=XJQVWKAN">“某个函数中定义的变量不能被另一个函数使用”</a></span>
3. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F4IHU78F5%22%2C%22annotationKey%22%3A%22NZ8UL3KT%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2258%22%2C%22position%22%3A%7B%22pageIndex%22%3A57%2C%22rects%22%3A%5B%5B201.994%2C114.6%2C453.994%2C129.36%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22locator%22%3A%2258%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/4IHU78F5?page=58&#x26;annotation=NZ8UL3KT">“用任意类型相符表达式初始化”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/I2QD5IEX">“LinuxC”</a></span>)</span>
4. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F4IHU78F5%22%2C%22annotationKey%22%3A%22UZER5RA4%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2260%22%2C%22position%22%3A%7B%22pageIndex%22%3A59%2C%22rects%22%3A%5B%5B331.012%2C418.35%2C547.012%2C433.11%5D%2C%5B46.012%2C404.202%2C454.012%2C418.11%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22locator%22%3A%2260%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/4IHU78F5?page=60&#x26;annotation=UZER5RA4">“初值可能不同”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/I2QD5IEX">“LinuxC”</a></span>)</span>
5. Scope ([“LinuxC”, p. 58](zotero://select/library/items/I2QD5IEX)) ([pdf](zotero://open-pdf/library/items/4IHU78F5?page=58&annotation=PZDAL2HG))








