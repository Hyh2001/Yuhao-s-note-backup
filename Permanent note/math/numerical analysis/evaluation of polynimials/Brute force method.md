For a [[polynomial]] $p_{n}(x) =a_{0}+a_{1}x+a_{2}x^{2}+\ldots +a_{n}x^{n}$ 
We can define $u_{k}=a_{0}+a_{1}x+\ldots +a_{k}x^{k}$ Then we can recursively compute :: $u_k=u_{k-1}+a_{k}x^{k}$. ([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=7&annotation=M5FQMCU9)) <!--SR:!2023-03-08,2,230-->
The key to this method is to store **the intermediate value**. $t_{k}=x^{k}$. Then $t_{k}=x\cdot t_{k-1}$   ([pdf](zotero://open-pdf/library/items/I5WT2TUR?page=8&annotation=RICLVU7C)) <!--SR:!2023-03-08,3,250-->

# multiplication times 
:: $2n$  <!--SR:!2023-03-08,3,250-->

