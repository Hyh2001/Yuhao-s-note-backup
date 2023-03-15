 #computer_science/programming_language/python #review 

## 表示
```python
[a,b,c,d]
```
## 类型转换
```python
list(A)
```
## 元素访问
### slicing
```python
A[n1,n2]
```
## 元素操作
### 修改元素
```python
A[a] = number
```
### 添加元素
#### append 
```python
A.append(x)
```
在list末尾添加元素x
#### insert
```python
A.insert(n,x)
```
在list的第n个元素后面插入x
### 删除元素
#### del
```python
del A[n]
```
删除list A的第n个元素
#### pop
```python
x = pop(A)  #弹出列表末尾元素
pop(number)  #弹出任意位置变量
```
#### remove
```python
 x = remove(' ') #删除指定值
```
### 排序
```python
A.sort(reverse = True) #按字母顺序排列，reverse参数为真则顺序相反
B = sorted(A)  #A的顺序不变
A.reverse()  #倒转顺序
```
## 列表操作
### 获取长度
```python
len(A) # 获取列表长度
```
### 遍历
```python
for n in A:
```
### 创建数值列表
#### 常规方法
```python
range(n1,n2,step)
```
#### 解析式
```python
A = [i for i... ]  #i符合的公式
```
### 复制
