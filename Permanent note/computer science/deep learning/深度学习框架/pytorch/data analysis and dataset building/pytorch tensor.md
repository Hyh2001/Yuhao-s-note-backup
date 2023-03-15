Pytorch 的基本数据结构是张量 Tensor。张量即多维数组。Pytorch 的张量和 numpy 中的 [[nadrray]] 很类似

创建一个tensor:
```python
i = torch.tensor(1) # 从一个数字创建一个tensor 
```
# tensor 的类型
1. troch.float64(torch.double)
2. torch.float32(torch.float) 这个是最常用的数据类型
3. torch.float16
4. torch.int64(torch.long)
5. torch.int32(torch.int)
6. torch.int16
7. torch.int8
8. torch.unit8
9. torch.bool
指定tensor的数据类型
```python
i = torch.tensor(1,dtype = torch.int32) #指定dtype参数
i = torch.IntTensor(1)
i = torch.FloatTensor(1)
i = torch.BoolTensor(1)
```
数据类型转化
```python
i.float() #使用float方法
i.type(torch.float) #使用type函数
i.type_as(a)  # 转换成和a tensor相同的类型
```
# tensor的维度
1. [[scalar]]为0维张量
2. [[vector]]为1维
3. [[matrix]]为2维
4. [[image]]加上了RGB三个通道为三维
5. 视频加上时间维为4维
## 判断维数方法
有几个中括号就是几维
{
```python 
tensor_name.dim() #返回一个tensor的维数
```
}
# tensor的尺寸
## 查看tensor的尺寸
```python
tensor_name.size()
tensor_name.shape 
```
## 改变tensor的尺寸
```python
tensor_name.view(a,b)  # a*b的矩阵
tensor_name.view(a,end) # end代表自动推断
tensor_name.reshape(a,b) # 变成a*b的矩阵
 ```
# tensor to [[nadrray]] and [[python list]] 
from_numpy 和numpy（）这两种方法关联的Tensor和numpy数组是共享数据内存的。 如果改变其中一个，另外一个的值也会发生改变。
```python 
import numpy as np 
import torch

tensor = torch.from_numpy(array) #此时你改变array的值，tensor的值也会随之增加
array = tensor.numpy() #改变 tensor,array 也会随之变化
array = tensor.clone().numpy() #改变 tensor,array 不会随之变化

scalar = torch.tensor(1.0)
s= scalar.item() # s变成了一个常量
t = tensor.tolist() # t变成了一个python list

```



https://pytorchmaster.com/2-1%2C%E5%BC%A0%E9%87%8F%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84/