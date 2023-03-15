#ros
Metapackages are specialized [[ROS package]](and catkin). They do not install files (other than their [[package.xml]] manifest) and they do not contain any tests, code, files, or other items usually found in packages.
A metapackage simply references one or more related packages which are loosely grouped together and packages them into a single logical package. 
# Structure of metapackages 
It likes a normal package with export tag in the package. xml: 
```xml
<export> 
  <metapackage />
</export>
```
It does not have build dependencies and only has execution dependencies. 
Its [[CMakelists.txt]] is like: 
```cmake 
cmake_minimum_required(VERSION 2.8.3)
project(<PACKAGE_NAME>)
find_package (catkin REQUIRED)
catkin_metapackage()
```
# How to create a metapackage? 







1. [Metapackages - ROS Wiki](http://wiki.ros.org/Metapackages)
2. [catkin/package.xml - ROS Wiki](http://wiki.ros.org/catkin/package.xml#Metapackages)