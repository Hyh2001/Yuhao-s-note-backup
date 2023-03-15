# header
```python
    import torch
	from torch import nn
```
# implementation
#todo （写的更加清晰）
继承Module类来构造神经网络（Module类是所有神经网络模块的基类）
代码
```python
Class MLP(nn.Module):
     def __init__(self,**kwargs):**​**
     super(MLP,self).__init__(**kwargs)
```
** 意味着将kwargs这个字典写成xi=ni的形式作为参 数传入， super（）方法用于调用父类的方法，而且只调用直接继承的父类
模型需要定义
