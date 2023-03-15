---
aliases: [rigid motion]
---
#robotics/robot_motion 

A rigid-body motion is a continuous movement of the particles in the object such that the distance between any two particles and orientation of the body remain fixed at all times. Accumulating rigid motions we can get [[rigid displacement]]. 

There are two major properties of rigid body motions. 
1. This motion preserves distance between points inside the rigid body. ($||p(t)-q(t)|| = ||p(0) - q(0)||$) (It is not sufficient to only follow this property, because [[reflection]] is also allowed.)
2. This motion preserves angles between vectors inside the rigid body.  ([[cross product]] is preserved: $g_*({v\times w}) = g_*({v})\times g_*({w})$ )

# representation of a rigid body's transformation 
We achieve the representation of the rigid body motion by attaching a [[reference frame]] to the body. We can represent this frame as a $4 \times 4$ matrix. It is an [[implicit representation]] method which $10$-constraints will be applied to the $16$-dimensional space of the matrix. The matrix is called [[homogeneous transformation matrix]]. 


# representation of a rigid body’s velocity
We can use [[spatial velocity]] to represent a rigid body's velocity.







1. rigid motion ([Murray 等, 1994, p. 40](zotero://select/library/items/YAI7PHQ7)) ([pdf](zotero://open-pdf/library/items/QG2EE4ZN?page=40&annotation=9UZC355R))
2. property 2 ([Murray 等, 1994, p. 42](zotero://select/library/items/YAI7PHQ7)) ([pdf](zotero://open-pdf/library/items/QG2EE4ZN?page=42&annotation=LVDBL9L5))