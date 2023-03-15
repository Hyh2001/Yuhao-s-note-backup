---
aliases: [squared error]
---
It is defined as :: $l^{(i)}(w, b)=\frac{1}{2}(\hat{y}^{(i)}-y^{(i)})^{2}$  <!--SR:!2023-03-14,6,230-->
([pdf](zotero://open-pdf/library/items/I3IXYM7V?page=126&annotation=UZFUU5BM))
# properties of this error 
1. large differences between estimates $\hat{y}^{(i)}$ and [[target]]  $y^{(i)}$ lead to **even larger contributions** to the loss, due to the quadratic form ([pdf](zotero://open-pdf/library/items/I3IXYM7V?page=126&annotation=HUHLJWXK))
	1. This encourages the model to avoid **large errors** 
	2. This leads to **excessive sensitivity to anomalous data**  <!--SR:!2023-03-26,14,250!2023-03-29,16,250!2023-03-14,6,230-->

# programming implementation 
```python 
loss = nn..MSELoss()
```