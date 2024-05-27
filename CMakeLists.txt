cmake_minimum_required(VERSION 3.10)

# Set the project name and version
project(RayTracing VERSION 1.0 LANGUAGES CXX)

# Specify the C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Add the src directory (if you have a CMakeLists.txt there in the future)
if(EXISTS ${CMAKE_SOURCE_DIR}/src)
    add_subdirectory(src)
endif()

# Add the test directory
add_subdirectory(test)
