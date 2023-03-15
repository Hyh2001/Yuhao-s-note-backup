#review 
# 局部变量和全局变量重名

```C
#include <stdio.h> 
int hour = 23, minute = 59; 
void print_time(void) {   
	printf("%d:%d in main\n",hour,minute); 
} 
int main(void){   
	int hour = 0, minute = 30;   
	print_time();   
	printf("%d:%d in main\n",hour,minute);   
	printf("x = %d\n",x);   
	 return 0;  
}
```
第一次调用 print_time 打印的是全局变量的值，第二次直接调用 printf 打印的则是 main 函数的局部变量的值。

标识符优先使用局部定义的，如果局部没有定义再使用全局的

# [[scope]]



1. <span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F4IHU78F5%22%2C%22pageLabel%22%3A%2258%22%2C%22position%22%3A%7B%22pageIndex%22%3A57%2C%22rects%22%3A%5B%5B58%2C262.452%2C548.5%2C276.36%5D%2C%5B46%2C246.6%2C130%2C261.36%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22locator%22%3A%2258%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/4IHU78F5?page=58">“global variable - local variable”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/I2QD5IEX">“LinuxC”</a></span>)</span>