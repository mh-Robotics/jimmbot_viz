cmake_minimum_required(VERSION 2.8.3)
project(jimmbot_viz)

add_compile_options(-std=c++17)

find_package(catkin REQUIRED COMPONENTS roslaunch)

catkin_package()

roslaunch_add_file_check(launch)

install( DIRECTORY launch rviz
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
