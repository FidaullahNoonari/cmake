cmake_minimum_required(VERSION 3.16.3)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# dir
set(CMAKE_INCLUDE_PATH ./include)

project(main VERSION 1.0)

add_executable(${PROJECT_NAME} main.cpp)

target_include_directories(${PROJECT_NAME} PUBLIC ./include)

add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/lib/addsub)

add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/lib/multdivide)

target_link_libraries(${PROJECT_NAME} addsub multdivide)
