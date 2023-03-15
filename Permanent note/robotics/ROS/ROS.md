#ros #todo 

ROS is a free and open source meta-operating system for robots that is used in both commercial and research applications. 
ROS has many functions and features (see [[ROS functions]]).  ([pdf](zotero://open-pdf/library/items/AZFGEHEQ?page=2&annotation=FLZLTWJ6))
## Why we need ROS?
It is because that ROS offers us a solution to divide the control software of robotics systems into various low-level, independent control loops that each manages a single task on the robot and couple the loops together with high-level logics. ([pdf](zotero://open-pdf/library/items/AZFGEHEQ?page=2&annotation=UDTTMZ3W))

# ROS architecture

[[ROS architecture]] is shown in the file. Through the architecture, data will flow between ROS nodes which can even be on different computers.

# ROS working space

Inside a working space, there are many folders and files. The structure and operations of the ROS working space is as follow. See ([[ROS working space]])

# ROS package

Inside the [[src folder]] of ROS working spaces, we can see [[ROS package]]s. They are the organization unit of ROS codes. The structure of ROS packages are as follow.(see ROS package) There is also a special ROS package called [[ROS metapackage]]. It is used to store multiple ROS package and group them.

# [[ROS node]]

We can build several nodes indies a package. ROS nodes are the smallest working units. Its structure can be seen in ROS node. Both [[rospy]] and [[roscpp]] have APIs for building nodes.


[[ROS file system]]

[[ROS computational concepts]]

[[ROS client libraries]]
[[ROS working space]]

[[ROS build system]]
[[ROS GUI tools]]

[[ROS command tools]]


# ROS installation 
## problems faced and solving 
1. ``` E: Malformed entry 1 in list file /etc/apt/sources. list. d/ros-latest. list (Component) The list of sources could not be read.```
	1. ```sudo rm /etc/apt/sources.list.d/ros-latest.list```
‍


