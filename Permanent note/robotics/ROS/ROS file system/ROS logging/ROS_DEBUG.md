#ros

DEBUG 是最低的级别，只在调试时使用，不会输出到控制台。我们可以编写程序打印需要的内容。有几种打印方式,Base 方式，Named方式，Conditional方式，Once方式，Throttle方式，Delayed throttle方式，Filter方式

# 打印ROS_DEBUG级别消息
```C++
#include <ros/console.h>
	// Base type, output to a logger named
	// "ros.<your_package_name"
		ROS_DEBUG( "word ", "after");
		ROS_DEBUG_STREAM("word " << "after");
	// Named type, output to a logger file named
	// "ros.<your_package_name>.name"
		ROS_DEBUG_NAMED("name","mid","last");
		ROS_DEBUG_STREAM_NAMED("name","mid"<<"last");
```
