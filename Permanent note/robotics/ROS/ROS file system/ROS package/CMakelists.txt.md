 #ros #cmake #review 

All the commands to build the ROS source code inside the package and create the executable. It is used by [[CMake]].

## CMakelist.txt for ROS packages

The basic structure of a CMakelists.txt file for [[ROS package]] is as follow.

```Cmake
cmake_minimum_required(VERSION number)
project(name_of_projet)
# find catkin and catkin packages
find_package(catkin REQUIRED)

# declare messages  and services
add_message_files(DIRECTORY msg FILES Num.msg)
add_service_files(DIREcTORY service FILES AddTwoInts.srv)

# generate messages and services
generate_message(DEPENDENCIES std_msgs)
catkin_package()

# build publisher and subscriber 
include_directories(include ${catkin_INCLUDE_DIRS})

add_executable(talker src/talker.cpp)
target_link_libraries(talker ${catkin_LIBRARIES})
add_dependencies(talker beginner_tutorials_generate_messages_cpp)

add_executable(listener src/listerner.cpp)
target_link_libraries(listener ${catkin_LIBRARIES})
add_dependencies(listener beginner_tutorials_generate_messages_cpp)
```
