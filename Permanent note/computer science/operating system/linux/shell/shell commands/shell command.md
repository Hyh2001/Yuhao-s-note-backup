# 命令格式
?
```shell 
命令名称  [命令参数/flag or options] [命令对象]
```
<!--SR:!2023-03-18,6,230-->

## 命令参数

### 长格式
?
```shell
man --help
```
不可合并 <!--SR:!2023-03-23,11,250-->

### 短格式
?
```shell
man -h
```
可以合并，“-”只需要保留一个 <!--SR:!2023-03-14,2,248-->

# 帮助命令
[[man]]

# input and output stream 
Input stream is for programs to **read input** and output stream is for program to **print something**. Normally both of the streams are on the **terminal**  <!--SR:!2023-03-14,2,248!2023-03-15,2,248-->

## change of streams 
### > and < 
?
```shell 
echo hello > hello.txt # will write hello into hello.txt 
cat < hello.txt # use hello.txt as the input of cat 
```
<!--SR:!2023-03-22,10,250-->

# [[shell pipe]]
