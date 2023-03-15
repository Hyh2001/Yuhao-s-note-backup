变量是计算机存储器中的一块命名的空间， 可以在里面存储一个值（Value），存储的值是可以随时变的。C语言中不同类型的变量所占用的存储空间大小是不同的，变量的最小存储单位是字节（[[byte]])。C变量的类型分别是字符型、整型、浮点型：
1.  char
2.  int
3.  float or double
# naming rules
必须以字母或下划线_（Underscore）开头，后面 可以跟若干个字母、数字、下划线，但不能有其它字符。
# variable definition 
定义一个变量，就是分配 一块存储空间并给它命名。
```C
int a; 
```
# [[assignment]]
给变量赋值
# [[initialization]]
变量的定义和赋值一步完成



1. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F4IHU78F5%22%2C%22annotationKey%22%3A%228M3CQLHN%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2238%22%2C%22position%22%3A%7B%22pageIndex%22%3A37%2C%22rects%22%3A%5B%5B318.244%2C674.85%2C546.244%2C689.61%5D%2C%5B46%2C659.85%2C364.756%2C674.61%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22locator%22%3A%2238%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/4IHU78F5?page=38&#x26;annotation=8M3CQLHN">“C variable”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/I2QD5IEX">“LinuxC”</a></span>)</span>
2. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F4IHU78F5%22%2C%22annotationKey%22%3A%222VFMHCX2%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2240%22%2C%22position%22%3A%7B%22pageIndex%22%3A39%2C%22rects%22%3A%5B%5B409.006%2C495.6%2C541.006%2C510.36%5D%2C%5B46.006%2C481.452%2C178.006%2C495.36%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22locator%22%3A%2240%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/4IHU78F5?page=40&#x26;annotation=2VFMHCX2">“variable definition”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/I2QD5IEX">“LinuxC”</a></span>)</span>
3. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F4IHU78F5%22%2C%22annotationKey%22%3A%22UXQ5UFW7%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2238%22%2C%22position%22%3A%7B%22pageIndex%22%3A37%2C%22rects%22%3A%5B%5B285.994%2C303.6%2C546.982%2C318.36%5D%2C%5B45.982%2C289.452%2C333.982%2C303.36%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22locator%22%3A%2238%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/4IHU78F5?page=38&#x26;annotation=UXQ5UFW7">“naming rule”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/I2QD5IEX">“LinuxC”</a></span>)</span>
