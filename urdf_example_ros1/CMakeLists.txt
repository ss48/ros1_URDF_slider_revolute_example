cmake_minimum_required(VERSION 3.0.2)
project(urdf_example)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  xacro
  robot_state_publisher
)

catkin_package()

include_directories(${catkin_INCLUDE_DIRS})

install(DIRECTORY launch urdf DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})

