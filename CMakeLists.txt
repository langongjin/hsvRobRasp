cmake_minimum_required(VERSION 3.6)
project(hsvRobRasp)

FIND_PACKAGE(OpenCV REQUIRED)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES main.cpp)
add_executable(hsvRobRasp ${SOURCE_FILES})

target_link_libraries(hsvRobRasp ${OpenCV_LIBS})