cmake_minimum_required(VERSION 2.8.3)

project(nxt_controllers)

find_package(catkin REQUIRED COMPONENTS
  nav_msgs
  nxt_msgs
  rospy
  sensor_msgs
  tf
  tf_conversions
)

find_package(orocos_kdl REQUIRED)

catkin_python_setup()

catkin_package(
  CATKIN_DEPENDS nav_msgs nxt_msgs rospy sensor_msgs tf tf_conversions
)
