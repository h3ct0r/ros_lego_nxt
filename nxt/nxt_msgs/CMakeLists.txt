cmake_minimum_required(VERSION 2.8.3)

project(nxt_msgs)

find_package(catkin REQUIRED COMPONENTS
  message_generation
  geometry_msgs
  std_msgs
)

add_message_files(FILES
  Accelerometer.msg
  Color.msg
  Contact.msg
  Gyro.msg
  JointCommand.msg
  Light.msg
  Sound.msg
  Range.msg
)

generate_messages(DEPENDENCIES
  geometry_msgs
  std_msgs
)

catkin_package(
  CATKIN_DEPENDS message_runtime
)
