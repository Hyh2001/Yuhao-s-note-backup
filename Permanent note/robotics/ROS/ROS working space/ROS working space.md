#ros 

ROS working space is consisted of several folders. Three folders are the most basic ones. [[build folder]], [[devel folder]] and [[src folder]]. For users we usually create [[install folder]] for convenience. The structure can be shown below: 
![[Pasted image 20230202040748.png]]

# Create a workspace
we can build a ROS working space by the commands mentioned below.  
```shell 
mkdir -p ~/catkin_ws/src 
cd ~/catkin_ws/  
catkin_make
```
Another choice is: 
```shell
mkdir -p ~/catkin_ws/src 
cd ~/catkin_ws/src  
catkin_init_workspace
```
# overlay of working space

We can also overlay working spaces. What is the overlay of working space? see [[overlay of working space]]. This technique is used for us to choose between which version of ROS packages we want to use. Based on overlay techniques, we can change between different working spaces in order to build projects individually.

# using multiple working spaces
```shell 
 source ~/overlay_ws/devel/setup.bash
```
 To change between different work spaces, we need to source them at first. And then we can directly use the work space.




1. Create workspace  ([pdf](zotero://open-pdf/library/items/AZFGEHEQ?page=5&annotation=J9QR4WPY))

1. 