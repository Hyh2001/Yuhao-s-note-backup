#review 
# 模型构造

直接在前向传播中定义
```python
class MLP(nn.Module):
		def __init__(self):  #定义需要的类和参数
 			super().__init__()
			self.hidden =
			self.out =

		der forward(self,X):  #定义前向计算
			return self out(F.relu(self.hidden(X)))
			# 使用这个类的方法：
			# net = MLP()
			# net(X)
```
另一种模型构造方法
使用sequential方法定义
```python
class Mysequential(nn.Module):
		def __init__(self,*args):
			super().__init__()
			for block in args:
				self._modules[block] = block
		def forward(self,X)
			for block in self._modules.values():
				X = block(x)
			return X
	net = Mysequential(nn.Linear(),nn.ReLU(),…)
```
两种定义方法可以嵌套使用

# 参数管理

## 获得单层的参数
```python
    net[n].state_dict()  #类型是OrderedDict
	net[n].bias #获得偏倚的完整情况
	net[n].bias.data #获得偏移的数据
	net[2].weight.grad #访问梯度

	#一次性访问所有参数
	*[(name,param.shape) for name, param in net.named_parameters()]
```

## 初始化

### linear
```python
net.apply(init_normal) #对于每一个module都调用这个方法
```

### 参数绑定（绑定几个层的参数）

```python
net.apply(init_normal) #对于每一个module都调用这个方法
```

# 自定义层

也是定义一个层类之后，将它实例化并把数据放进去

## 传入参数
```python
def __init __(self,in_units,units):
		super().__init__()
		self.para =nn.Parameter(torch.random(in_units,units))
```
