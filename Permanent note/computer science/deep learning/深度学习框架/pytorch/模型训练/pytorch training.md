?
```python

num_epochs = 

for epoch in range(epochs):
	for X,y in Dataloader：
		l = loss(net(X),y)
		trainer.zero_grad()
		l.backward()
		trainer.step()
	l = loss(net(features),labels)
	print(f'epoch{epoch+1},loss{l:f}')
```
<!--SR:!2023-03-09,1,210-->