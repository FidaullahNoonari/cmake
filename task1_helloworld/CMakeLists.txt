cmake_minimum_required(VERSION 3.16.3)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(hello_world)

add_executable(${PROJECT_NAME} main.cpp)