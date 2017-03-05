# Dependencies
 ros-teleop

# launch gazebo simulator
 roslaunch mybot_gazebo mybot_world.launch
# launch RViz 
 roslaunch mybot_description mybot_rviz.launch
 fix frame to odometry frame
 add robot model
# Gazebo movement
## move by keyboard
 rosrun teleop_twist_keyboard teleop_twist_keyboard.py
## move automatically 
 rostopic pub /cmd_vel geometry_msgs/Twist
 circle mode: set velocity linear.x = 0.3 and angular.z = 0.1
