cmake_minimum_required(VERSION 2.8)

project(ad3)

# Set build flags
#set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fPIC")

#set(EIGEN_DIR "${CMAKE_SOURCE_DIR}/../Eigen)")
set(AD3_DIR "${CMAKE_SOURCE_DIR})")

#include_directories(${EIGEN_DIR})
include_directories(${AD3_DIR})

file(GLOB_RECURSE SRC "*.h" "*.cpp")
#file(SRC Factor.h Factor.cpp)
add_library(${PROJECT_NAME} ${SRC})