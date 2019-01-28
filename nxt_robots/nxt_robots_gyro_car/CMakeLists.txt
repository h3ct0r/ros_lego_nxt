cmake_minimum_required(VERSION 2.8.3)

project(nxt_robots_gyro_car)

find_package(catkin REQUIRED COMPONENTS
nxt_controllers
 nxt_description
 nxt_ros
 robot_pose_ekf
 robot_state_publisher
)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES nxt_robot_gyro_car
  CATKIN_DEPENDS nxt_controllers nxt_description nxt_ros robot_pose_ekf robot_state_publisher
#  DEPENDS system_lib
)