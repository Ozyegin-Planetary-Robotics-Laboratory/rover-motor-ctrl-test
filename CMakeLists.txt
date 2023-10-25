cmake_minimum_required(VERSION 3.0.2)
project(rover-motor-ctrl-test)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
  std_msgs
  message_generation
)

catkin_package(
        #  INCLUDE_DIRS include
        #  LIBRARIES neo6m-ros
        #  CATKIN_DEPENDS roscpp std_msgs
        #  DEPENDS system_lib
        CATKIN_DEPENDS roscpp rospy std_msgs message_runtime
)

include_directories(
        # include
        ${catkin_INCLUDE_DIRS}
)

catkin_install_python(PROGRAMS
  scripts/main.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)