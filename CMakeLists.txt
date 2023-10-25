cmake_minimum_required(VERSION 3.0.2)
project(<OZU_PACKAGE_NAME>)


catkin_install_python(PROGRAMS
  src/main.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)