#computer_science/programming_language/C  
C语言的语句和低级语言的指令之间并不是简单的一一对应的关系。一条语句会翻译成多条汇编指令或者机器指令，这个过程叫作编译（[[compile]]），由编译器（[[compiler]]）完成。
**C语言的语句和低级语言语句之间并不是一一对应的**
# C 语言优点
1. C语言写出来的代码更加紧凑，可读性更强，也更容易改正。
2. C语言是可移植的（portable），与平台(platform)无关。这里的平台可以指计算机体系结构（[[architecture]]）也可以指操作系统（[[operating system]])。 这个优点是因为C编译器可以把程序编译成该计算机自己的机器指令(native)， 所有C语言程序只要稍微修改就可以在别的计算机上运行。
# [[C program structure]]
# How to read a C program  
按照代码的执行顺序进行阅读，首先需要阅读的是[[main function]]  <!--SR:!2023-03-15,3,250-->









1. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F4IHU78F5%22%2C%22annotationKey%22%3A%22V4I29Q87%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2222%22%2C%22position%22%3A%7B%22pageIndex%22%3A21%2C%22rects%22%3A%5B%5B190%2C459.6%2C511%2C474.36%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22locator%22%3A%2222%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/4IHU78F5?page=22&#x26;annotation=V4I29Q87">“C语言”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22itemData%22%3A%7B%22id%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%2C%22type%22%3A%22book%22%2C%22title%22%3A%22LinuxC%22%7D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/I2QD5IEX">“LinuxC”</a></span>)</span>
2. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F4IHU78F5%22%2C%22annotationKey%22%3A%22EVGEB9LQ%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2222%22%2C%22position%22%3A%7B%22pageIndex%22%3A21%2C%22rects%22%3A%5B%5B358.732%2C354.6%2C538.732%2C369.36%5D%2C%5B45.976%2C339.6%2C543.232%2C354.36%5D%2C%5B45.976%2C324.6%2C543.976%2C339.36%5D%2C%5B45.976%2C309.6%2C545.476%2C324.36%5D%2C%5B45.976%2C294.6%2C273.976%2C309.36%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22locator%22%3A%2222%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/4IHU78F5?page=22&#x26;annotation=EVGEB9LQ">“C 语言优点”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22itemData%22%3A%7B%22id%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%2C%22type%22%3A%22book%22%2C%22title%22%3A%22LinuxC%22%7D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/I2QD5IEX">“LinuxC”</a></span>)</span>
3. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F4IHU78F5%22%2C%22annotationKey%22%3A%22B6A9CR26%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2251%22%2C%22position%22%3A%7B%22pageIndex%22%3A50%2C%22rects%22%3A%5B%5B428.5%2C633.702%2C548.5%2C647.61%5D%2C%5B46%2C618.702%2C286%2C632.61%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22locator%22%3A%2251%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/4IHU78F5?page=51&#x26;annotation=B6A9CR26">“how to read C program”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/I2QD5IEX">“LinuxC”</a></span>)</span>
‍