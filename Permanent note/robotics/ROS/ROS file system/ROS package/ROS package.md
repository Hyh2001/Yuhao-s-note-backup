#ros
ROS package contains all source code ([[ROS node]]), data files, build files, dependencies, and other files are organized in packages. It is used to organize ROS code into logical units and manage their dependencies. 
# structure

ROS package contains several components. It contains [[CMakelists.txt]], folders:  [[include]], [[package.xml]], [[src]], [[script]], [[msg]], [[srv]], [[launch]], [[lib]].
# create ROS package
We can follow the steps and codes below to create a ROS package.

```bash
	cd ~/catkin_ws/src
	catkin_create_pkg name [depend1] [depend2] [depend3]
	# usually the three depends are std_msgs,rospy,roscpp
	cd ~/catkin_ws
	catkin_make
	source catkin_ws/devel/setup.bash
```
 ([pdf](zotero://open-pdf/library/items/AZFGEHEQ?page=5&annotation=K7MHXTXX))
# reveal of dependencies of a ROS package

ROS dependencies are stored in [[package.xml]], you can see the dependencies inside the folder. The dependencies of the package can also have dependencies which are named [[indirect dependency]],

# Shell command for ROS packages 
[[rospack]]


# Use of non-built-in package  
If you want to use a non-built-in package, you will need to source the setup. bash file inside the [[devel folder]]  for that package’s workspace.
```shell 
source workspace_name/devel/setup.bash
```
 ([pdf](zotero://open-pdf/library/items/AZFGEHEQ?page=6&annotation=YZHKIXG5))