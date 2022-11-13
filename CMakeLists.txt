# cmake needs this line
cmake_minimum_required(VERSION 3.1)

set(CMAKE_C_COMPILER "gcc")
set(CMAKE_CXX_COMPILER "g++")

add_definitions(-D_GNU_SOURCE)
# Define project name
project(libcssl VERSION 0.0.0 LANGUAGES C CXX)


# be set, you can find the full list with descriptions

# Declare the executable target built from your sources
add_executable(${PROJECT_NAME} test.c cssl.c)



