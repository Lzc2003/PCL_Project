cmake_minimum_required(VERSION 2.6 FATAL_ERROR)
project(KD_TREE)
find_package(PCL 1.3 REQUIRED)
include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})
add_executable(KD_SEARCH kdtree_search.cpp)
target_link_libraries(KD_SEARCH ${PCL_LIBRARIES})

