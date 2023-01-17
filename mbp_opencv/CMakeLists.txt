cmake_minimum_required(VERSION 3.24)
project(mbp_opencv)

set(CMAKE_CXX_STANDARD 11)

find_package(OpenCV)

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(mbp_opencv main.cpp)

target_link_libraries(mbp_opencv ${OpenCV_LIBS})