cmake_minimum_required(VERSION 2.8.3)
project(rqt_smach)

find_package(catkin REQUIRED)

catkin_python_setup()

catkin_package()

install(
  FILES plugin.xml
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

catkin_install_python(
  PROGRAMS scripts/${PROJECT_NAME}
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
