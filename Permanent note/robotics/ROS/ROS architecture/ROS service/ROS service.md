#ros #review 

The ROS Service is used to pass data between nodes and it uses Request/Reply mechanism to achieve it. It is used between [[server node]] and [[client node]]. [[client node]] will require ROS service offered by [[server node]] with arguments and may receive some responds. There are several commands used for us to get information and modify services in terminals.

# rosservice
```shell
	# 1. show all the services 
	rosservice list 
	# 2. find out the type of a services 
	rosservice type [name]
	# 3. call a service 
	rosservice call [name] [args]
```
# build own service file
We can also build our own service types. The implementation is as follow:
1. see [[srv file]]


1. ROS service ([pdf](zotero://open-pdf/library/items/AZFGEHEQ?page=10&annotation=EHZISXAR))