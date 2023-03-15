#ros 

## roscore

```shell
roscore
```

start Ros master + rosout +parameter server

### features

run roscore on one terminal window, and use another terminal window to enter the next command to run a ROS node

#### a better way

install terminator for opening multiple terminals at the same time

## rosed
```shell
rosed [package_name] [filenames]
```
Allows you to directly edit a file within a package by using the package name rather than having to type the entire path to the package.

### tab completion
```shell
rosed [package_name]<tab><tab>
```
see and optionally edit all files from a package without knowing its exact name.
```shell
rosed [package_name]<tab><tab>
```
see and optionally edit all files from a package without knowing its exact name

## rosnode
```shell
rosnode [parameters] [name] 
```
explore all the aspects of a ROS node
```shell
rosnode [parameters] [name]
```
explore all the aspects of a ROS node
```shell
	# 1. show the lists of nodes running on the system  
	rosnode list  
	# 2. Display information about a node, including publications and subscriptions  
	rosnode info name  
	# 3. rearranging node name  
	rosrun package node_name:=name
```
## rostopic
```shell
rostopic [parameters] [name]
```
provides information about the topics publishing/subscribing in the system
```shell
	# 1. print topic message
		rostopic echo name
	# 2. publish a topic with data
		rostopic pub -r topic_name msg_type data
		# -r means publishing rate in HZ
	# 3. print information about active topic
		rostopic list
	# 4. display bandwidth used by topics (the bandwidth reported is the received bandwidth)
		rostopic bw name
	# 5. display publishing rate of topic
		rostopic hz
	# 6. print topic type
		rostopic type
```

## rosmsg
```shell
	rosmsg show name
```

### message file
message file: simple text files that describe the fields of a ROS message

### structure
```yaml
	Header header
	string ...
```