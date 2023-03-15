#review  
函数声明的结构如下:
```C
返回值类型 函数名(参数列表);
```
声明提供给 [[compiler]] 的信息只有函数名和返回值类型. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F4IHU78F5%22%2C%22annotationKey%22%3A%22URW6A9MW%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2252%22%2C%22position%22%3A%7B%22pageIndex%22%3A51%2C%22rects%22%3A%5B%5B416.5%2C494.202%2C548.5%2C508.11%5D%2C%5B46%2C479.202%2C178%2C493.11%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22locator%22%3A%2252%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/4IHU78F5?page=52&#x26;annotation=URW6A9MW">“function declaration”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/I2QD5IEX">“LinuxC”</a></span>)</span>
# 函数声明作用
它为编译器提供了有用信息，编译器在处理代码的过程中，只有见到函数原型（不管带不带函数体）之后才知道这个函数的名字、参数类型和返回值，然后在碰到函数调用时才知道怎么生成相应的指令，所以函数原型必须出现在函数调用之前，这也是遵循“先声明后使用”的原则。([“LinuxC”, p. 51](zotero://select/library/items/I2QD5IEX)) ([pdf](zotero://open-pdf/library/items/4IHU78F5?page=51&annotation=I8LZUT7P))

# [[function implicit declaration]]



