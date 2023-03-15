#ros #review 
ROS node is the process that use ROS APIs to perform computations. It is simply an executable file. Nodes exchange control messages, sensor readings, and other data by publishing or subscribing to [[ROS topic]] or by sending requests to [[ROS service]]  offered by other nodes

There are four types of ROS nodes: [[publisher node]], [[subscriber node]], [[client node]], [[server node]]. The nodes are created by using [[ROS client libraries]].  After finishing programming a node, we need to write Ros [[CMakelists.txt]] and using catkin_make to compile it. The preliminaries of using ROS nodes is to open the [[ROS master]] at first.

# ROS node commands

We can perform works like listing active nodes, providing information of nodes, running nodes and etc.
## list active nodes
```shell 
# 1. to see all the nodes 
	rosnode list 
```
## provide information of nodes 
```shell 
# 2. to print out information of a node 
	rosnode info name
```



1.  ROS node ([pdf](zotero://open-pdf/library/items/AZFGEHEQ?page=3&annotation=PEMYIDH6))
2. Function of ROS nodes ([pdf](zotero://open-pdf/library/items/AZFGEHEQ?page=3&annotation=C5QCW4V6))