```python 
loss.backward(retain_graph = True) # 计算图在反向传播后立即销毁，如果需要保留计算图, 需要设置retain_graph = True
```