![[Pasted image 20220926205757.png]]
Its structure includes [[ROS master]], [[ROS node]]s, [[ROS topic]]s and [[ROS message]]s. Message transferring process will be controlled by ROS master. Two way are used to transfer ROS messages.

1. The first way is to use [[publisher node]] and [[subscriber node]]. ROS messages will be wrapped in [[ROS topic]]s. Then the messages will be sent from publisher node to subscriber node.
2. The second way is to use [[server node]] and [[client node]]. Client node will send message to call for [[ROS service]]s. Server node will execute the service and give back the results in the form of ROS messages.

‍