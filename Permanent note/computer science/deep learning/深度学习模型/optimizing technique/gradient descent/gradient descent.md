It is the method that iteratively reducing the error by **updating the parameters in the direction that incrementally lowers the [[loss function]]**. ([pdf](zotero://open-pdf/library/items/I3IXYM7V?page=128&annotation=6T47CIEE)) <!--SR:!2023-03-15,7,250-->

# steps of gradient descent 
1. Taking the [[derivative]] of the loss function 
2. Passing over **the entire** data set 
3. update parameters  <!--SR:!2023-03-16,8,250-->

# drawbacks of gradient descent 
1. It is extremely **slow** 
2. If there is a lot of **redundancy** in the training data, the benefit of a full update is even lower 
	* [ ] what does redundancy means in the context? 
([pdf](zotero://open-pdf/library/items/I3IXYM7V?page=128&annotation=JJLA5N9J)) <!--SR:!2023-03-24,12,250!2023-03-16,8,250-->

## solutions 
1. [[stochastic gradient descent]]
2. [[minibatch stochastic gradient descent]]