# Robot Force Torque Sensor - How Does It Work?

![rw-book-cover](https://readwise-assets.s3.amazonaws.com/static/images/article0.00998d930354.png)

## Metadata
- Author: [[Mathieu Bélanger-Barrette]]
- Full Title: Robot Force Torque Sensor - How Does It Work?
- Category: #articles
- URL: https://blog.robotiq.com/bid/72444/Robot-Force-Torque-Sensor-How-does-it-work

## Highlights
- Most robotic applications require a multi-axis or 6-axis FT sensor to give feedback to the robot about the tool itself which can be controlled along 6 axes (3 translations + 3 rotations). A 6-axis FT sensor means that the sensor can measure both the force and torque along the 3-axis (x-y-z). These are usually defined by the components of Fx-Fy-Fz and Tx-Ty-Tz. To measure the effort in all six axes, the force-torque sensor usually combines information from a minimum of 6 unitary measuring elements such as strain gauges. Using the geometry of these elements and the physical properties of the material on which they are installed, we can compute the force and torque along the axes which are meaningful to the robot control loop. When installed on the robot flange, the integrator needs to set the parameters for the relative position and orientation of the sensor with respect to the robot tool.
- Some FT sensors use gauges that digitize the measurement from the start, getting rid of the possibility of electromagnetic noise sensitivity interference, which is an issue experienced with traditional strain gauges.
