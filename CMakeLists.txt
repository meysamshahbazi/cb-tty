# cmake needs this line
cmake_minimum_required(VERSION 3.1)

set(CMAKE_C_COMPILER "gcc")
set(CMAKE_CXX_COMPILER "g++")
add_definitions(-D_GNU_SOURCE)
# Define project name
project(libcssl VERSION 0.0.0 LANGUAGES C CXX)

# Find OpenCV, you may need to set OpenCV_DIR variable
# to the absolute path to the directory containing OpenCVConfig.cmake file
# via the command line or GUI

# If the package has been found, several variables will
# be set, you can find the full list with descriptions
# in the OpenCVConfig.cmake file.
# Print some message showing some of them

# Declare the executable target built from your sources
add_executable(${PROJECT_NAME} test.c cssl.c)

# Link your application with OpenCV libraries


