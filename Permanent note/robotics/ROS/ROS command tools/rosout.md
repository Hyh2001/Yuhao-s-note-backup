rosout is the name of the console log reporting mechanism in ROS. It can be thought as comprising several components:
1. The rosout node for subscribing, logging, and republishing the messages.
2. The /rosout topic
3. The /rosout_agg topic for subscribing to an aggregated feed. (==what is an aggregated feed?==) #todo 
4. rosgraph_msgs/Log message type, which defines standard fields as well as verbosity levels. 
5. Client APIs facilitate easy use of the rosout reporting mechanism.
6. GUI tools, like rqt_console, for viewing the console log messages.


1. [rosout - ROS Wiki](http://wiki.ros.org/rosout)