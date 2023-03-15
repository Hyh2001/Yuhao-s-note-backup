The space Jacobian connects the [[angular velocity]] and [[spatial twist]]. $V_{s}=J_{s}(\theta)\dot{\theta}$. 
Each column $J_{si}(\theta)=Ad_{e^{S_{1}\theta_{1}}\ldots e^{[S_{i-1}]\theta_{i-1}}}(S_{i})$ corresponds to a [[screw axis]] expressed in the fixed [[space frame]] $\{s\}$. 
([Lynch 和 Park, 2017, p. 197](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=197&annotation=3JQRZ6KB))

# physical meaning 
$S_{i}$ is the screw axis describing the $i-th$ joint axis in terms of the zero position of the robot. Therefore  $Ad_{e^{S_{1}\theta_{1}}\ldots e^{[S_{i-1}]\theta_{i-1}}}(S_{i})$ represents the $i-th$ joint axis after it undergoes previous $i-1$ rigid body transformations which is $J_{si}(\theta)$. In summary, the $J_{si}(\theta)$ is the screw vector expressed in fixed-frame coordinates for arbitrary $\theta$ 
([Lynch 和 Park, 2017, p. 198](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=198&annotation=BM2FUN4J))

# derivation 
From the [[product of exponential]] equations we know that $T (\theta_{1},\theta_{2},\ldots,\theta_{n})=e^{[S_{1}]\theta_{1}}e^{[S_{2}]\theta_{2}}\ldots e^{[S_{n}]\theta_{n}}M$. 
We can [[differentiate]] both sides versus $t$:
$$
\begin{aligned}
\dot{T} & =\left(\frac{d}{d t} e^{\left[\mathcal{S}_1\right] \theta_1}\right) \cdots e^{\left[\mathcal{S}_n\right] \theta_n} M+e^{\left[\mathcal{S}_1\right] \theta_1}\left(\frac{d}{d t} e^{\left[\mathcal{S}_2\right] \theta_2}\right) \cdots e^{\left[\mathcal{S}_n\right] \theta_n} M+\cdots \\
& =\left[\mathcal{S}_1\right] \dot{\theta}_1 e^{\left[\mathcal{S}_1\right] \theta_1} \cdots e^{\left[\mathcal{S}_n\right] \theta_n} M+e^{\left[\mathcal{S}_1\right] \theta_1}\left[\mathcal{S}_2\right] \dot{\theta}_2 e^{\left[\mathcal{S}_2\right] \theta_2} \cdots e^{\left[\mathcal{S}_n\right] \theta_n} M+\cdots
\end{aligned}
$$
We can also [[transpose]] $T$

$$
T^{-1}=M^{-1} e^{-\left[\mathcal{S}_n\right] \theta_n} \cdots e^{-\left[\mathcal{S}_1\right] \theta_1} .
$$
We know that $[V_{s}]=\dot{T}T^{-1}$, we can get
$$
\left[\mathcal{V}_s\right]=\left[\mathcal{S}_1\right] \dot{\theta}_1+e^{\left[\mathcal{S}_1\right] \theta_1}\left[\mathcal{S}_2\right] e^{-\left[\mathcal{S}_1\right] \theta_1} \dot{\theta}_2+e^{\left[\mathcal{S}_1\right] \theta_1} e^{\left[\mathcal{S}_2\right] \theta_2}\left[\mathcal{S}_3\right] e^{-\left[\mathcal{S}_2\right] \theta_2} e^{-\left[\mathcal{S}_1\right] \theta_1} \dot{\theta}_3+\cdots .
$$
The above can also be expressed using [[adjoint representation of special Euclidean group]] 
$$\mathcal{V}_s=\underbrace{\mathcal{S}_1}_{J_{s 1}} \dot{\theta}_1+\underbrace{\operatorname{Ad}_{e^{\left[\mathcal{S}_1\right] \theta_1}}\left (\mathcal{S}_2\right)}_{J_{s 2}} \dot{\theta}_2+\underbrace{\operatorname{Ad}_{e^{\left[\mathcal{S}_1\right] \theta_1} e^{\left[\mathcal{S}_2\right] \theta_2}}\left (\mathcal{S}_3\right)}_{J_{s 3}} \dot{\theta}_3+\cdots$$
Observe that $\mathcal{V}_s$ is a sum of $n$ spatial twists of the form
$$
\mathcal{V}_s=J_{s 1}+J_{s 2}(\theta) \dot{\theta}_1+\cdots+J_{s n}(\theta) \dot{\theta}_n
$$
where each $J_{s i}(\theta)=\left(\omega_{s i}(\theta), v_{s i}(\theta)\right)$ depends explicitly on the joint values $\theta \in \mathbb{R}^n$ for $i=2, \ldots, n$. In matrix form,
$$
\begin{aligned}
\mathcal{V}_s & =\left[\begin{array}{llll}
J_{s 1} & J_{s 2}(\theta) & \cdots & J_{s n}(\theta)
\end{array}\right]\left[\begin{array}{c}
\dot{\theta}_1 \\
\vdots \\
\dot{\theta}_n
\end{array}\right] \\
& =J_s(\theta) \dot{\theta} .
\end{aligned}
$$
([Lynch 和 Park, 2017, p. 197](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=197&annotation=UP5NWK4C))