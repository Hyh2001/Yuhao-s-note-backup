#ros

ROS topic is a message bus or path where [[ROS message]] s passing through it. The messages are published by [[publisher node]] and received by [[subscriber node]]. Each topic has a name. 

It has several terminal commands to help users working on ROS topic.  There is also a tool called [[Rqt_graph]] to help us better understanding relationships between nodes and topics. The commands are as follow

# rostopic
```shell
	# 1. To see the available sub-commands
	rostopic -h
	# 2. Display bandwidth used bu topics
	rostopic bw
	# 3. Print message to screen
	rostopic echo [name]
	# 4. Display publishing rate of topics
	rostopic hz
	# 5. Print information about active topics
	# -v will include the message type used for each topic 
	rostopic list -v
	# 6. publish data to topic
	rostopic pub topic msg_type arts
	# 7. print topic type
	rostopic type
```




1. ROS topic ([pdf](zotero://open-pdf/library/items/AZFGEHEQ?page=8&annotation=HKEUP48N))