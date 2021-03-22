cmake_minimum_required(VERSION 3.0.2)
project(sick_safetyscanners_description)

find_package(catkin REQUIRED COMPONENTS)

catkin_package()

install(DIRECTORY meshes urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
