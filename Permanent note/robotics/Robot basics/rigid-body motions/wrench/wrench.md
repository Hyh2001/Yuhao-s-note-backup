---
aliases: [spatial force]
---
It is made of **a [[force]] and a [[torque]]** which merges them together into a six-dimensional vector expressed in the [[frame]] $\{a\}$ . we denoted it as $F_{a}=\begin{bmatrix}m_{a}\\f_{a}\end{bmatrix}\in\mathbb{R}^{6}$  ([Lynch 和 Park, 2017, p. 127](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=127&annotation=LJ8CSZ64))
[[pure moment]] 

# transformation between different wrenches 
The relationships are listed below: 
$F_{b}=Ad_{T_{ab}}^T(F_{a})$ where $Ad$ means the :: [[adjoint representation of special Euclidean group]]. 
([Lynch 和 Park, 2017, p. 128](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=128&annotation=ZKSG99R3))
## proof 
We can proof the equation by using the [[conservation of energy principle]]. 
The [[dot product]] of velocity and [[force]] is the [[power]]. 
$V_{b}^TF_{b}=V_{a}^{T}F_{a}$ where $V$ is [[twist]] 
We know that for twist $V_{a}=Ad_{T_{ab}}V_b$ and we plug it in the previous equation. 
$V_{b}^{T}F_{b}=V_{b}^{T}Ad_{T_{ab}}^T (F_{a})$ and finally we get  $F_{b}=Ad_{T_{ab}}^T(F_{a})$
 ([Lynch 和 Park, 2017, p. 127](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=127&annotation=FR9XSA2K))