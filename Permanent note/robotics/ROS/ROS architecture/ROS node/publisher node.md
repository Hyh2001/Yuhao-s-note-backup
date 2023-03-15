#ros 

Publisher node is the node that used to send data. It sends [[ROS message]]  to a [[ROS topic]]. Then the [[subscriber node]] will receive the data. There are two ways which based on [[rospy]] and [[Roscp]] APIs for building a publisher node.

# structure of a publisher node

1. init a node with args
2. build a node handler
3. set the publish topic name and messgae type
4. set loop rate
5. publish message and loop

## Roscpp api
```cpp
#include "ros/ros.h"      //  includes all the headers necessary to use the most common public pieces of the ROS system
#include "std_msgs/String.h" // include message that you want to use
int main(int arc, char *argv)
{
/* argc
   argv*/
	ros::init(argc, argv, "name", options);  // 1. allows ROS to do name remapping through the command line. 2. Specify the name of the node which should be unique in a running system. 
	ros::NodeHandle n; // create a handle to this process node. The first hadle will initialize the whole node, the last one destructed will clean up all the resources used. 
	ros::Publisher chatter_pub = n.advertise<std_msgs::String>("chatter", 1000);  // 
	    // 1. std_msgs::String is the type of message we want to publish 
	    // 2. chatter is the topic we publish our message in
	    // 3. 1000 is the size of publishing queue which means that if we publish data too quickly, the system will buffer up to 1000 messgages. 
	    // 4. NodeHandle::advertise() serves for two purpose: (1) it contains pulish() method that lets you publish messages onto the topic. (2) when goes out of scope, it will automatically unadvertise 
	ros::Rate loop_rate(10);
	//specify a frequency that you would like to loop at. Unit is Hz
	while (ros::ok())
	{  //ros::ok() will be false in 4 conditions
	   // 1. Ctrl-C. 
	   // 2. kicked off by another same node 
	   // 3. ros::shutdown() has been called 
	   // 4. All ros::NodeHandles have been destroyed
		std_msgs::String msg;

		std::stringstream ss;
		ss << "hello world"; 
		msg.data = ss.str();
		// create the message 
		// add sleep here 
		chatter_pub.publish(msg);
		//publish the message 

		ros::spinOnce();
		loop_rate.sleep();
	}
}
```

## Rospy api
```python
import rospy 
from std_msgs.msg import String 

def talker():
	pub = rospy.Publisher('chatter', String, queue_size =10)
	rospy.init_node("talker", anonymous = True)
	rate = rospy.Rate(10)
	while not rospy.is_shutdown():
		hello_str = "hello world %s" % rospy.get_time() 
		rospy.loginfo(hellp_str)
		pub.publish(hello_str)
		rate.sleep()

if __name__ == "__main__":
	try:
		talker()
	except rospy.ROSInterruptException:
		pass
```

## Problems involved in programming  
1. 发布者前几条数据可能丢失: 注册后加入休眠，
```C++
ros::Duration(3.0).sleep()
```
2. 