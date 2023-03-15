#robotics/robot_motion 

Twist is a six-dimensional velocity vector which merges **[[angular velocity]]  $\omega$ and [[linear velocity]] $v$** relative to a [[frame]]. ([Murray 等, 1994, p. 40](zotero://select/library/items/YAI7PHQ7)) ([pdf](zotero://open-pdf/library/items/QG2EE4ZN?page=40&annotation=TUZ6B48X))

$V = \begin{bmatrix} \omega \\ v \end{bmatrix} \in \mathbb{R}^6$ or $V = \begin{bmatrix} v \\ \omega \end{bmatrix} \in \mathbb{R}^6$  ([[Does it matter whether v is in the front for twists？]])

Twists can be divided into [[body twist]] and [[spatial twist]].
And they can be simplified for both pure rotations and pure translations 
1. Pure rotation: $V = \begin{bmatrix} -\omega \times q \\ \omega \end{bmatrix}$ ([pdf](zotero://open-pdf/library/items/9ZMQK9KL?page=55&annotation=QDL7TIR3))  ([Pardos-Gotor, 2021, p. 28](zotero://select/library/items/V6J2RZZH))
2. Pure translation: $V = \begin{bmatrix} v \\ 0 \end{bmatrix}$ ([pdf](zotero://open-pdf/library/items/9ZMQK9KL?page=55&annotation=GZRY6G9V))  ([Pardos-Gotor, 2021, p. 28](zotero://select/library/items/V6J2RZZH))
## relationship between different twists

We use [[adjoint representation of special Euclidean group]] to transform between different twists. 
$\begin{bmatrix} R & 0 \\ [p]R & R \end{bmatrix}$

# screw interpretation of twist

As stated in [[Chasles-Mozzi theorem]], a twist can be interpreted in terms of a [[screw axis]] $S$ and a rotation velocity $\dot{\theta}$ about the axis.  Then we can represent a twist as:

$V = \begin{bmatrix} w \\ v \end{bmatrix} = \begin{bmatrix} \vec{s}\dot{\theta} \\ -\vec{s}\dot{\theta} \times q + h\vec{s}\dot{\theta}     \end{bmatrix}$



## proof
see [[Chasles-Mozzi theorem]]

## normalized twist

$[S] = \begin{bmatrix} [\omega] & v \\ 0 & 0\end{bmatrix}$ where $[\omega]$ is the skew-symmetrical representation of $\omega$ 

## transformation of screw axis
$S_a = [Ad_{T_{ab}}]S_b$


# programming implementation

```matlab
% find the skew-symmetric form of a twist
se3mat = VecTose3(V)
% find the twist from skew-symmetric form
V =se3ToVec(se3mat)
% find the screw representation of a twist from q,s,h
S = ScrewToAxis(q,s,h)
% find screw axis and distance traveled from exponential coordinate
[S,theta] = AxisAng(expc6)

```



1. [robotics - Excerpt of: Lynch_Park_2017_Modern robotics, p120](lt://open/pHy13yu7oU2oGOec55gOOA)


