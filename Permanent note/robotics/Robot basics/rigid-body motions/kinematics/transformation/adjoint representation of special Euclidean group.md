Given a transformation matrix $T \in SE(3)$, we can define adjoint representation as $[Ad_T]$ which is: 

$[Ad_T] = \begin{bmatrix} R & 0 \\ [p]R & R \end{bmatrix} \in \mathbb{R}^{6 \times 6}$ and $V^{'} = [Ad_{T_{V^{'}V}}]V = Ad_T(V)$ 
$[p]$ is the [[skew-symmetric matrix]] of $p$ 
This representation is used to transform between [[body twist]] and [[spatial twist]]. 
## derivation 
$[V_s] =\begin{bmatrix} \omega_s \\ v_s \end{bmatrix} = T[V_b]T^{-1} = \begin{bmatrix} R & 0 \\ [p]R & R \end{bmatrix} \begin{bmatrix} \omega_b \\ v_b \end{bmatrix}\in \mathbb{R}^{6 \times 6}$

## properties of adjoint representation

1. Let $T_1$, $T_2 \in SE(3)$ and $V = (\omega,v)$. Then $Ad_{T_1}(Ad_{T_2}(V)) =Ad_{T_1T_2}(v)$
2. $[Ad_T]^{-1} = [Ad_{T^{-1}}]$, we can prove it by setting $T_1 = T_2^{-1}$ in property 1.
