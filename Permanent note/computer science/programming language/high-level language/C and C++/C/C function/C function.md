C 函数的结构如下：
1. 返回值类型：规定了返回的变量的类型 (若没有返回值则使用 void )
2. 函数名规定了函数的名字，它遵循 [[identifier]] 的命名规则
3. 参数列表：规定了传入参数的个数和类型。
4. 语句列表：用来实现功能以及返回返回值（return value）
```C
返回值类型 函数名（参数列表）
{
	语句列表;
}
```
# 函数调用
函数调用是使用函数的过程，它的语句类似于：
```C
a = sin(x)
```
$a$ 被称作返回值
$x$ 被称作参数（[[C parameter]]（形参），[[C argument]]（实参））
$sin(x)$ 即被称作函数调用

函数调用也是一种表达式（[[expression|statement]]）。这个表达式由函数调用运算符（也就是括号）和操作数组成。
# C 函数特点
1. 函数可以被多次调用
2. 函数的调用可以嵌套
# C 函数 side effect
函数执行的过程中还会改变一些存储的数据或进行输入输出操作。

# C 函数定义和声明
1. 函数声明（[[function declaration]]）
2. 函数定义 ([[function definition]])
3. 函数原型 ([[function prototype]]) 

# 特殊的函数
1. [[main function]]








1. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F4IHU78F5%22%2C%22annotationKey%22%3A%22DXZISX97%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2247%22%2C%22position%22%3A%7B%22pageIndex%22%3A46%2C%22rects%22%3A%5B%5B526.756%2C300.6%2C538.756%2C315.36%5D%2C%5B46.012%2C286.452%2C538.012%2C300.36%5D%2C%5B46.012%2C270.6%2C535.75%2C285.36%5D%2C%5B45.994%2C255.6%2C540.262%2C270.36%5D%2C%5B46.006%2C240.6%2C100.762%2C255.36%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22locator%22%3A%2247%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/4IHU78F5?page=47&#x26;annotation=DXZISX97">“C 函数调用”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/I2QD5IEX">“LinuxC”</a></span>)</span>， 
2. C 函数调用 2([“LinuxC”, p. 47](zotero://select/library/items/I2QD5IEX)) ([pdf](zotero://open-pdf/library/items/4IHU78F5?page=47&annotation=DXZISX97))
3. Side Effect([“LinuxC”, p. 47](zotero://select/library/items/I2QD5IEX)) ([pdf](zotero://open-pdf/library/items/4IHU78F5?page=47&annotation=TDGIX8JG))
4. C 函数特点 ([“LinuxC”, p. 51](zotero://select/library/items/I2QD5IEX)) ([pdf](zotero://open-pdf/library/items/4IHU78F5?page=51&annotation=IIXPJJRA))