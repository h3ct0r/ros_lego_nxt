cmake_minimum_required(VERSION 2.8.3)

project(nxt_ros_test)

find_package(catkin REQUIRED COMPONENTS
  nxt_ros
  rospy
)

# catkin_python_setup()

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES nxt_ros_test
 CATKIN_DEPENDS nxt_ros rospy
#  DEPENDS system_lib
)