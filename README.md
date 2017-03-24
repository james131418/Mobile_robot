# Dependencies
 1. catkin
 2. mybot_control
 3. mybot_description - contains URDF of mybot
 4. mybot_gazebo

# launch Gazebo simulator
 roslaunch mybot_gazebo mybot_world.launch
 ![gazebo](https://cloud.githubusercontent.com/assets/18408973/23586218/c07ec580-015e-11e7-9097-dd4df9bb0cb6.png)
# launch RViz 
 1. roslaunch mybot_description mybot_rviz.launch
 2. fix frame to odometry frame
 3. add robot model
 ![rviz](https://cloud.githubusercontent.com/assets/18408973/23586238/083f2554-015f-11e7-8950-7bbd02c692cb.png)

# Robot motion in Gazebo
## move by keyboard
 rosrun teleop_twist_keyboard teleop_twist_keyboard.py
## move automatically 
rostopic pub /cmd_vel geometry_msgs/Twist
* circle mode: set velocity linear.x = 0.2 and angular.z = 0.1
