It uses a series connection of a spring([[Hooke's law]]) and a dashpot elements([[Newton's law of viscosity]]) ([pdf](zotero://open-pdf/library/items/PXFCS2FM?page=13&annotation=ZGSHSB8G))
![[Pasted image 20230312172132.png]]

# derivation
Because it is series model: 
1.  [[stress]] on each element is the same. $\sigma_s=\sigma_d$ 
2. Total [[strain]] equals to the sum of strains of each elements.  $\epsilon = \epsilon_{s}+\epsilon_{d}$. We [[differentiate]] both sides and get: 
$\dot{\epsilon}=\frac{\dot{\sigma_s}}{E}+\frac{\sigma_{d}}{{\mu}}$  
## for [[stress relaxation]] 
Because the [[strain rate]] will be $\dot{\epsilon}=0$, we can have :: $\sigma(t)=\sigma_{0}e^{\frac{-E}{\mu}t}$ ($\sigma_{0}=\sigma_{s}=\sigma_{d}$) ([pdf](zotero://open-pdf/library/items/PXFCS2FM?page=13&annotation=U4KTEUVT))  
## for [[creep]] 
We have a constant stress rate which means that $\dot{\sigma}=0$. We can have :: $\epsilon(t)=\frac{\sigma}{\mu}t+\epsilon_{0}$ ([pdf](zotero://open-pdf/library/items/PXFCS2FM?page=13&annotation=8K2NRJAD)) 
([pdf](zotero://open-pdf/library/items/9A3RFKZQ?page=1&annotation=G34DR57H))    

# drawbacks 
1. cannot predict viscous recovery and decreasing strain rate creep 
2. can predict [[elastic]] response and a permanent strain  
([pdf](zotero://open-pdf/library/items/PXFCS2FM?page=13&annotation=YN2R6GN3))