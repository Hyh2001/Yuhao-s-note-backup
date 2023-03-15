#ros #review 

A program that normally runs along with the [[ROS master]]. The user can store various parameters or values on this server and all the [[ROS node]] can access it. The user can set privacy of the parameter too. If it is a public parameter, all the nodes have access to it; if it is private, only a specific node can access the parameter. We can list parameters, add parameters, modify parameters, delete parameters dump parameters to file, load parameters from files and etc.  There are also several commands for us to modify the parameters on the server.
# rosparam

```bash
	# 1. set a parameter 
	rosparam set [name]
	# 2. get a parameter 
	rosparam get [name]
	# 3. write parameters to a file
	rosparam dump [file_name] [namespace]
	# 4. load parameters from file
	rosparam load [file_name] [namespace]
	# 5. delete a parameter 
	rosparam delete [name]
```
