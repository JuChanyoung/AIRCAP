cmake_minimum_required(VERSION 2.8.3)
project(uav_msgs)

find_package(catkin REQUIRED message_generation std_msgs nav_msgs geometry_msgs)

add_message_files(
  FILES
  uav_pose.msg
)

generate_messages(DEPENDENCIES std_msgs nav_msgs geometry_msgs)

catkin_package(
  CATKIN_DEPENDS message_runtime std_msgs nav_msgs geometry_msgs
)

