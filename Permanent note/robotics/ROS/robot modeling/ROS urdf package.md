It is the [[ROS package]] used to **model robots**. It contains a paerser for the [[unified robot description format|URDF]] file. It has several components: 
1. urdf_parser_plugin: This package implements methods to **fill URDF data structures**. 
2. urdfdom_headers: This component provides core data structure headers to use the urdf parse
3. collada_parser: This package populates data structures by parsing a Collada file
4. urdfdom:  This component populates data structures by parsing URDF files
5. collada-dom: This is a stand-alone component to convert Collada documents with 3D computer graphics software such as Maya, Blender, and Soft image 
Despite the packages that processing the URDF file itself, we can also use packages to interact between URDF files and other packages: 
1. joint_state_publisher: This package contains a node called joint_state_publisher, which reads the robot model description, finds all joints, and publishes joint values to all nonfixed joints using GUI sliders. The user can interact with each robot joint using this tool and can visualize using RViz. While designing URDF, the user can verify the rotation and translation of each joint using this tool.
2. kdl_parser: : It is a component of the [[kinematic and dynamics library]]. 
3. robot_state_publisher: This package reads the current robot joint states and publishes the 3D poses of each robot link using the kinematics tree build from the URDF. The 3D pose of the robot is published as the tf (transform) ROS. The tf ROS publishes the relationship between the coordinates frames of a robot.
4. [[xacro]]: define how xacro is equal to URDF plus add-ons. It contains some add-ons to make URDF shorter and readable, and can be used for building complex robot descriptions. We can convert xacro to URDF at any time using ROS tools.
 ([Joseph 和 Cacace, 2018, p. 73](zotero://select/library/items/MMUP6DDD)) ([pdf](zotero://open-pdf/library/items/4H7JC8DI?page=91&annotation=KGEXPB65))