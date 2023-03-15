#ros 

ROS launch file is a [[xml]] file. The structure of a ROS launch file can be seen as follow.
![[Pasted image 20221001140341 2.png]]
![[Pasted image 20221001140404.png]]
# ROS launch file structure
```xml
	<launch>      <!-- launch 标签充当其它标签的容器 -->
	deprecated = "弃用声明"    <!-- 表示launch文件已经被弃用-->
		<group ns = "name">   <!-- this allow us to build a namespace. With which we can run a node in the same name without confliction -->
			<node pkg = "pkg_name" name = "sim" type = "turtlesim_node">
		</group>
	</launch>     <!--斜杠为从左下到右上-->

```