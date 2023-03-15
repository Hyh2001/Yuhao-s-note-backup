#computer_science/programming_language/C  
Escape sequences are some [[string literal]]s that do not show their original meanings. 转义序列有两个作用：一是把普通字符转义成 特殊字符，例如把字母n转义成换行符；二是把特殊字符转义成普通字符，例如\和"是特殊字符，转义后取它的字面值。
Types of escape sequences are listed below: 
```c
\'  // 单引号 
\"  // 双引号
\?  // 问号
\\  // 反斜线
\a  // 响铃, 喇叭发出滴的一声
\b  // 退格， 和按下退格键效果一样
\f  // 分页符， 控制打印源代码时提前分页
\n  // 换行， windows和网络协议很多用\n,\r作为换行符，但是linux只使用\n作为换行符
\r  // 回车
\t  // 水平制表符， 和按下TAB键效果相同
\v  // 垂直制表符， 在终端下定位表格的下一列
```


[[C format string - escape sequence]]



1. ([“LinuxC”, p. 34](zotero://select/library/items/I2QD5IEX)) ([pdf](zotero://open-pdf/library/items/4IHU78F5?page=34&annotation=9V2GNR4D))