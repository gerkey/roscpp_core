project(roscpp_core)
cmake_minimum_required(VERSION 2.8)
find_package(catkin)
find_package(genmsg)

foreach(subdir
    cpp_common
    rostime
    roscpp_traits
    roscpp_serialization
    )
  add_subdirectory(${subdir})
endforeach()

catkin_package(roscpp_core)
