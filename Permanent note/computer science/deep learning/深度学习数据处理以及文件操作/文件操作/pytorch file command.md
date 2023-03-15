
# 加载和保存向量

```python
torch.save (x,’file name’)
A = torch.load(‘file name’)
```

## 存储张量列表

```python
torch.save([x,y],’file name’)
```

## 存储字典

```python
torch.save(dict,’file name’)
```

# 加载和保存模型

```python
torch.save(net.state_dict(),’file name.params’).   #模型中的所有参数存成一个字典
```

## 加载模型

```python
Clone = net()
Clone.load_state_dict(torch.load(‘file name.Paramus’))
```
