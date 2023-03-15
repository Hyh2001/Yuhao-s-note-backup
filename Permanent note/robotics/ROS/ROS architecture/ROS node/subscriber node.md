#ros

subscriber node is the node that will subscribe to the topic published by a [[publisher node]]. There are two ways which based on [[rospy]] and [[roscpp]] APIs for building a subsciber node.

# Roscpp implementation

```cpp
#include "ros/ros.h"
#include "std_msgs/String.h"

int main(int argc, char **argv)
{
	ros::init(argc, argv, "name");
	ros::NodeHndle n; 

	ros::Sbuscriber sub = n.subscribe(“chatter”,1000,chatterCallback);
	/*
	1. “chatter” is the topic that the subscriber listen to 
	2. Messages will be passed to the callback function “chatterCallback”. 
	3. 1000 is the length of the buffer queue. 
	
	*/
	ros::spin();
	/* 
	ros::spin() enters a loop, calling message callbacks as fast as possible
	It is exit When ros::ok() is false
	*/
	return 0;
}
void chatterCallback(const std_msgs::String::ConstPtr& msg)
{
	ROS_INFO(“I heard: [%s]”, msg -> data.c_str());
	
}
```


    ‍
