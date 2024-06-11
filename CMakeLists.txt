# Minimum required version of CMake
cmake_minimum_required(VERSION 3.10)

# Project name
project(Satellite-Simulation)

# Set C++ standard
set(CMAKE_CXX_STANDARD 11)

# Add source files using the proper directory structure
file(GLOB SOURCE "Source/*.cpp")

# Add header files
include_directories(Headers)

link_directories(Headers)

# Add executable target
add_executable(Satellite-Simulation ${SOURCE})

# Include header files
target_include_directories(Satellite-Simulation PUBLIC Headers)
