#review 
Screw axis is used to define a [[twist]]. We need three parameters to define a screw axis $S$ which are :: $\{q, \vec{s}, h\}$. $q \in \mathbb{R}^3$ is an arbitrary point on the axis, $\vec{s}$ is the unit vector in the direction of the axis and $h$ is the [[screw pitch]].

However, we do not want to represent the screw axis in this way,

1. If $\omega \neq 0$ , then:: $S = V/||\omega||$ which is simply $V$ normalized by the length of the angular velocity vector. (now $v = - \omega \times q + h\omega$) Then we can have $S\dot{\theta} = V$ for $||\omega|| = \dot{\theta}$
2. If $\omega = 0$ (pure translation, $h = \infty$) then :: $S = V/||v||$ which is simply $V$ normalized by the length of the linear velocity vector. Then we can have $S\dot{\theta} = V$ for $||v|| = \dot{\theta}$

==We can see from the definition above, if a twist is defined versus a frame {a}, its screw will also be represented versus the frame {a}== 
