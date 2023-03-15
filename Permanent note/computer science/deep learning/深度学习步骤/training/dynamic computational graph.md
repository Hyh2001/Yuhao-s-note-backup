# properties 
1. 计算图的正向传播是**立即执行**的。无需等待完整的计算图创建完毕，每条语句都会在计算图中动态添加节点和边，并立即执行正向传播得到计算结果。
2. 计算图在[[backpropagation]]后**立即销毁**。下次调用需要重新构建计算图。如果在程序中使用了backward方法执行了反向传播，或者利用torch.autograd.grad方法计算了梯度，那么创建的计算图会被立即销毁，释放存储空间，下次调用需要重新创建。
[[pytorch dynamic computational graph]] 

https://pytorchmaster.com/2-3%2C%E5%8A%A8%E6%80%81%E8%AE%A1%E7%AE%97%E5%9B%BE/