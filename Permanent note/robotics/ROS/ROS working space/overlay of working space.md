Overlaying refers to building and using a [[ROS package]] from source on top of an existing version of that same package.(==用于选择希望使用的ROS package==)

# command

```shell
source ~/overlay_ws_overlay/devel/setup.bash
	# original command is like
source /opt/ros/noetic/setup.bash
```

# principle

ROS会解析.bashrc文件，并生成ROS_PACKAGE_PATH ROS包路径，.bashrc文件中，后配置的优先级更高
