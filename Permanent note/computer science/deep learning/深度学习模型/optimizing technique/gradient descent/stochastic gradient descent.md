---
aliases: [SGD]
---
This methods update parameters after considering **only one** example.  ([pdf](zotero://open-pdf/library/items/I3IXYM7V?page=128&annotation=L7TSUCL3)) <!--SR:!2023-03-17,5,210-->

# drawbacks 
1. It takes **a lot longer** to process one sample at a time compared to a full batch ([pdf](zotero://open-pdf/library/items/I3IXYM7V?page=128&annotation=24BQI8JI))
2. Some of layers ([[batch normalization]]) only work well when having access to **more than one observations.** <!--SR:!2023-03-17,9,250!2023-03-27,15,250-->

# pytorch implementation 
```python
trainer = torch.optim.SGD(net.parameters(), lr =)
```
