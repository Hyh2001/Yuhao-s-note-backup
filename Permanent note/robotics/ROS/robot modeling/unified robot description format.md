---
aliases: [URDF]
---
It is a [[XML]] file used to **represent a robot**. It is used by the [[ROS urdf package]] to describe the **[[kinematics]], inertial properties and link geometry** of robots. . ([Joseph 和 Cacace, 2018, p. 73](zotero://select/library/items/MMUP6DDD)) ([pdf](zotero://open-pdf/library/items/4H7JC8DI?page=91&annotation=CQK45XIE)) ([Lynch 和 Park, 2017, p. 170](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=170&annotation=6CHARARK))

# structure of URDF 
## joints parameters 
1. two links connected to the joint: parent link and child link. ([Lynch 和 Park, 2017, p. 170](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=170&annotation=J5XLMSQJ))
2. joint types: 
	1. [[prismatic joint]] 
	2. [[revolute joint]] 
	3. continuous joint (**revolute joint without limits**)
	4. fixed joint (a virtual joint that **dose not permit any motion**) 
	  ([Lynch 和 Park, 2017, p. 170](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=170&annotation=6IW2MBQ4))
 3. frames: 
	 1. An origin frame defines **the position and orientation of the child link frame relative to the parent link frame when the joint variable is zero**. (It uses the [[roll pitch yaw angle]] to represent rotation) It is on the joint's axis. ([Lynch 和 Park, 2017, p. 170](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=170&annotation=QEBNK296))
	 2. An [[unit vector]] of 3 expressed in the child link's frame. It is **in the direction of positive rotation for a revolute joint or positive translation for a prismatic joint.**  ([Lynch 和 Park, 2017, p. 170](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=170&annotation=T83B36EK))
### the urdf of a joint
([Lynch 和 Park, 2017, p. 173](zotero://select/library/items/CK6BYIEW)) ([pdf](zotero://open-pdf/library/items/97TQKNC2?page=173&annotation=RG2FC8LQ))
```xml 
<joint name = "name" type = "type name">
	<parent link = "link_name1"/>
	<child link = "link_name2"/>
	<origin rpy = "0.0,0.0,0.0" xyz = "0.0,0.0,0.0"/>
	<axis xyz = "0,0,0"/>
</joint> 
``` 

## link parameters 
