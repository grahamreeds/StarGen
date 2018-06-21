cmake_minimum_required(VERSION 2.8)

project(StarGen)

# Set the output folder where your program will be created
set(CMAKE_BINARY_DIR ${CMAKE_SOURCE_DIR}/bin)
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_BINARY_DIR})
set(LIBRARY_OUTPUT_PATH ${CMAKE_BINARY_DIR})

# The following folders and sources will be included
include_directories(${CMAKE_SOURCE_DIR})
file(GLOB PROJECT_SOURCES "./*.c")

# The final executable
add_executable(StarGen ${PROJECT_SOURCES})