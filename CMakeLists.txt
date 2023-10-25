cmake_minimum_required(VERSION 3.0.2)
project(rover-motor-ctrl-test)


catkin_install_python(PROGRAMS
  src/main.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)