

# 查看GPU状态

```python
import torch
from torch import nn

# to see whether GPU is available
print(torch.cuda.is_available())

# how many GPUs are available
print(torch.cuda.device_count())

# soure GPU
torch.cuda.current_device()

# get the name of GPUs
torch.cuda.get_device_name(0)
```
# Tensor在GPU上计算

## 原理

创建一个**Device**并把可用的 GPU 放进去，然后用这个创建好的东西存储用于训练的数据 <!--SR:!2023-03-26,13,230-->

## 单块GPU

```python
# 创建GPU对象
device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")

# 训练数据
features = features.to(device)
labels = labels.to(device)

# 模型数据
net.to(device)
```
