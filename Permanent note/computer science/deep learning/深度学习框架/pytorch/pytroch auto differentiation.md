The pytorch has implemented the [[auto differentiation]] mechanism inside it.  

Pytorch一般通过
1. 反向传播 backward 方法 实现这种求梯度计算。该方法求得的梯度将存在对应自变量张量的grad属性下。 
2. 调用torch.autograd.grad函数来实现求梯度计算。
# backward 方法
## 标量反向传播
{
```python 
import numpy np 
import torch 

x = torch.tensor(0.0,requires_gad = True) # requires_gad 表示需要被求导
a = torch.tensor(1.0) 
b = torch.tensor(-2.0) 
c = torch.tensor(1.0) 
y = a*torch.pow(x,2) + b*x + c

y.backward() # 计算y对于变量的偏导 
dy_dx = x.grad # x.grad 获得y关于x的梯度

```
}
## 非标量反向传播
{
```python
import numpy as np 
import torch 
x = torch.tensor([[0.0,0.0],[1.0,2.0]],requires_grad = True) # x需要被求导 
a = torch.tensor(1.0) 
b = torch.tensor(-2.0) 
c = torch.tensor(1.0) 
y = a*torch.pow(x,2) + b*x + c 

gradient = torch.tensor([[1.0,1.0],[1.0,1.0]])
y.backward(gradient = gradient) 
x_grad = x.grad 
```
}
## 非标量反向传播通过标量方法实现
{
```python
import numpy as np import torch 
x = torch.tensor([[0.0,0.0],[1.0,2.0]],requires_grad = True) # x需要被求导 
a = torch.tensor(1.0) 
b = torch.tensor(-2.0) 
c = torch.tensor(1.0) 
y = a*torch.pow(x,2) + b*x + c 

gradient = torch.tensor([[1.0,1.0],[1.0,1.0]]) 
z = torch.sum(y*gradient)  
z.backward() 
x_grad = x.grad 
```
}
# autograd.grad 
{
```python
import numpy as np 
import torch 
x = torch.tensor([[0.0,0.0],[1.0,2.0]],requires_grad = True) # x需要被求导 
a = torch.tensor(1.0) 
b = torch.tensor(-2.0) 
c = torch.tensor(1.0) 
y = a*torch.pow(x,2) + b*x + c 

dy_dx = torch.autograd.grad(y,x,create_graph=True)[0]

# 多个变量求导
x1 = torch.tensor(1.0,requires_grad = True) # x需要被求导 
x2 = torch.tensor(2.0,requires_grad = True) 
y1 = x1*x2 
y2 = x1+x2 
(dy1_dx1,dy1_dx2) = torch.autograd.grad(outputs=y1,inputs = [x1,x2],retain_graph = True) 

# 多个因变量
(dy12_dx1,dy12_dx2) = torch.autograd.grad(outputs=[y1,y2],inputs = [x1,x2])
```
}
# 利用[[pytorch optimizer]]自动微分
{
```python
import numpy as np 
import torch 
x = torch.tensor(0.0,requires_grad = True) # x需要被求导 
a = torch.tensor(1.0)
b = torch.tensor(-2.0) 
c = torch.tensor(1.0) 

optimizer = torch.optim.SGD(params=[x],lr = 0.01) 
def f(x): 
	result = a*torch.pow(x,2) + b*x + c 
	return(result) 
for i in range(500): 
	optimizer.zero_grad() 
	y = f(x) 
	y.backward() 
	optimizer.step()
```
}

https://pytorchmaster.com/2-2%2C%E8%87%AA%E5%8A%A8%E5%BE%AE%E5%88%86%E6%9C%BA%E5%88%B6/
