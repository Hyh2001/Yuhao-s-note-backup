#ros 

An srv file describes a service. Its name is like "name.srv" It is composed of two parts: a request and a response. They are used to generate source code for a new type of services. These files are stored in [[srv]] in [[ROS package]]. The structure of it is as follow:

# structure

A srv file is just simple text files with a field type and field name per line. A srv file contains of two parts: a request and a response. The two parts are separated by "---" lines.

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
int64 A    #request
int64 B
---
int64 Sum   #response
```

# turned srv file into source code

### modify [[package.xml]] file

Add the code below (uncomment them)

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
  
add_service_files(
  FILES
  service.srv
)  

generate_messages(
  DEPENDENCIES
  std_msgs
)
```


([ros tutorial](http://wiki.ros.org/ROS/Tutorials/CreatingMsgAndSrv))
