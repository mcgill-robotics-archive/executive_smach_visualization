cmake_minimum_required(VERSION 2.8.3)

project(smach_viewer)

find_package(catkin REQUIRED COMPONENTS rostest)

catkin_package(
  CATKIN_DEPENDS smach_msgs smach_ros xdot
)

# Install targets
install(
  PROGRAMS scripts/${PROJECT_NAME}.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
