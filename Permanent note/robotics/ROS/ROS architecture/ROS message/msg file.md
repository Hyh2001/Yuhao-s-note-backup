#ros

Msg files are simple text files that describe the fields of a [[ROS message]]. Its name is like "name.msg" They are used to generate source code for messages in different languages. msg files are stored in the [[msg]]  of a [[ROS package]]. The structure of a msg file is as follow:

# structure

This file is just simple text files with a field type and field name per line. field type and field name specify the parameter that will be used when coding.

## field types
```yaml
int8, int16, int32, int64 (plus uint*)
float32, float64
string
time, duration
other msg files
variable-length array[] and fixed-length array[C]
Header
```
### Header
header contains a timestamp and coordinate frame information that are commonly used in ROS.

```yaml
  Header header
  string child_frame_id
  geometry_msgs/PoseWithCovariance pose
  geometry_msgs/TwistWithCovariance twist
```
# turned msg file into source code
### modify [[package.xml]] file
Add the code below

```XML
<build_depend>message_generation</build_depend>  <exec_depend>message_runtime</exec_depend>
```
### modify [[CMakelists.txt]] file

Add the code below:

1. modify the find_package method
2. modify catkin_package method
3. add add_message_files method
4. uncomment generate_messages method

```Cmake
find_package(catkin REQUIRED COMPONENTS
   roscpp
   rospy
   std_msgs
   message_generation
)

catkin_package(
  ...
CATKIN_DEPENDS message_runtime ...
  ...)
  
add_message_files(
  FILES
  Num.msg
)  

generate_messages(
  DEPENDENCIES
  std_msgs
)
```



([ros tutorial](http://wiki.ros.org/ROS/Tutorials/CreatingMsgAndSrv))
