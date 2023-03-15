The formula $\tau = \mu\frac{du}{dy}$ is called the Newton's law of viscosity and $\mu$ is called [[dynamic viscosity]] 

# derivation 

![[Pasted image 20230217192442.png]]
We can construct a theme where there are two plates inside a fluid and the upper plate moves a constant speed $V$ under the influence force $F$. This moving plate will exert a shear force on the fluid contacting with it and due to the [[no-slip condition]] the fluid in contact will also have a speed $V$. 
Then we can define the [[Permanent note/mechanical engineering/materials/soft materials/polymer/rheology/deformation force/shear stress]] as $\tau = \frac{F}{A}$ where $A$ is the contact area between the plate and the fluid. ([“fluid mechanics fundamentals and applications”, p. 51](zotero://select/library/items/TWA5RBHQ)) ([pdf](zotero://open-pdf/library/items/8J59SQQB?page=78&annotation=WAHJQ57X))
In steady and laminar flow (see [[steady flow]] and [[laminar flow]]), the velocity of fluid between two plates varies linearly from $0$ to $V$. We can thus define its [[velocity profile]] : 
$u (y) = \frac{y}{l}V$ where $l$ is the distance between two plates. we [[differentiate]] both sides will get $\frac{du}{dy} = \frac{V}{l}$ ([“fluid mechanics fundamentals and applications”, p. 52](zotero://select/library/items/TWA5RBHQ)) ([pdf](zotero://open-pdf/library/items/8J59SQQB?page=79&annotation=MMAVNYNI))  
For an infinitesimal interval of time $dt$ the move of fluid particles in contact with the upper plate can be treated as a rotation along point $M$. We can then calculate the [[shear strain]] as: 
$d\beta \simeq tan (d\beta) = \frac{Vdt}{l} = \frac{du}{dy}dt$ (the $\simeq$ has utilized the property of [[tan(x)]]) ([“fluid mechanics fundamentals and applications”, p. 52](zotero://select/library/items/TWA5RBHQ)) ([pdf](zotero://open-pdf/library/items/8J59SQQB?page=79&annotation=KHAUHNPM))
We thus proved that $\frac{d\beta}{dt} = \frac{du}{dy}$ which means that the [[strain rate]] is equivalent to the velocity profile. 