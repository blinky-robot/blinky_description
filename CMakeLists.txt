cmake_minimum_required(VERSION 2.8.3)
project(blinky_description)

find_package(catkin REQUIRED COMPONENTS
  urdf
)

###################################
## catkin specific configuration ##
###################################
catkin_package()

#############
## Install ##
#############

## Mark other files for installation (e.g. launch and bag files, etc.)
install(DIRECTORY
  urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
