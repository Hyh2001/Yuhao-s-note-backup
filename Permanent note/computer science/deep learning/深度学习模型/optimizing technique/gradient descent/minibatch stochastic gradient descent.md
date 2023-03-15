It is a combination of [[stochastic gradient descent|SGD]] and [[gradient descent]]. It takes a minibatch $B_i$ ([[batch_size]] is $|B|$) of observations which is between **32 ad 256 (a multiple of a large power of 2 will be better)**. 
([pdf](zotero://open-pdf/library/items/I3IXYM7V?page=128&annotation=ZMBDNA82))
# steps 
1. It computes the [[gradient]] of [[loss function]] of each examples in the minibatch and average then. 
2. Multiply the result by the [[learning rate]] and substract the result from model parameters. The equation is ::  $(w, b)-\frac{\eta}{|B|}\sum_{i \in B_{i}}\partial_(w,b)l^{(i)}(w,b)$ <!--SR:!2023-03-22,10,230-->
([pdf](zotero://open-pdf/library/items/I3IXYM7V?page=128&annotation=UTR986HC))