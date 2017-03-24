# Dependencies
1. catkin_make
2. mybot_gazebo
3. mybot_description -- contains URDF and rviz launch
4. mybot_control
5. mybot_navigation -- contains map and amcl navigate launch
# Using the ROS Navigation Stack
1. roslaunch mybot_gazebo mybot_world.launch
2. roslaunch mybot_navigation amcl_demo.launch
3. roslaunch mybot_description mybot_rviz_amcl.launch



