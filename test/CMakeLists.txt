cmake_minimum_required(VERSION 2.8)
project(jsoncpp_test)

if(CMAKE_CXX_COMPILER_ID STREQUAL GNU)
  set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
endif()

add_definitions(-Dprivate=public)
add_executable(jsoncpp_test unit.cpp)
include_directories(../src)
