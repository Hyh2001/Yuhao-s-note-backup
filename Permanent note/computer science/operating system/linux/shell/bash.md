---
aliases: [Bourne Again SHell]
---
# main interface 
```shell 
missing:~$
```
~ means that it is now in **home folder**
$ means that you are not **root user** <!--SR:!2023-03-20,8,248!2023-03-15,2,247-->

# command 
You can type in command inside the shell which will be interpreted. 
## execute a program 
```bash 
missing:~$ date # type in the name of the program 
```
## execute a command with argument 
```shell
missing:~$ echo hello # name of command [argument]
# argument with whitespace "My space" or My\ space
```
## special words in shell 
$? 是 Shell 中的一个特殊变量，表示**上一个运行结束的程序的退出状态**  <!--SR:!2023-03-15,2,247-->

<span class="highlight" data-annotation="%7B%22attachmentURI%22%3A%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2F4IHU78F5%22%2C%22annotationKey%22%3A%22X236KVLE%22%2C%22color%22%3A%22%23ffd400%22%2C%22pageLabel%22%3A%2249%22%2C%22position%22%3A%7B%22pageIndex%22%3A48%2C%22rects%22%3A%5B%5B46%2C376.35%2C409%2C391.11%5D%5D%7D%2C%22citationItem%22%3A%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%2C%22locator%22%3A%2249%22%7D%7D" ztype="zhighlight"><a href="zotero://open-pdf/library/items/4IHU78F5?page=49&#x26;annotation=X236KVLE">“$?”</a></span> <span class="citation" data-citation="%7B%22citationItems%22%3A%5B%7B%22uris%22%3A%5B%22http%3A%2F%2Fzotero.org%2Fusers%2F9667514%2Fitems%2FI2QD5IEX%22%5D%7D%5D%2C%22properties%22%3A%7B%7D%7D" ztype="zcitation">(<span class="citation-item"><a href="zotero://select/library/items/I2QD5IEX">“LinuxC”</a></span>)</span>
# principle of shell 
Shell is a programming environment and it has variables, conditionals, loops, and functions. When you run commands in your shell, you are really writing **codes** that your shell interprets.<!--SR:!2023-03-13,5,228-->

# [[shell path]] 





[Course overview + the shell · Missing Semester (mit.edu)](https://missing.csail.mit.edu/2020/course-shell/)