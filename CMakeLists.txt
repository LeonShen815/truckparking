cmake_minimum_required(VERSION 2.8.3)
project(truckparking)

## Find catkin and any catkin packages
find_package(catkin REQUIRED COMPONENTS)

## Declare catkin package
catkin_package()

## Build includes
include_directories(
    ${catkin_INCLUDE_DIRS}
    )

## Install other resources
install(
    DIRECTORY
    launch
    rviz
    urdf
    DESTINATION
    ${CATKIN_PACKAGE_SHARE_DESTINATION}
    )
