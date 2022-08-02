cmake_minimum_required(VERSION 3.16.3)  # CMake version check
project(Json_Library)               # Create project "simple_example"

set(CMAKE_CXX_STANDARD 17)            # Enable c++14 standard
set(CMAKE_CXX_STANDARD_REQUIRED True) 
set(CMAKE_BUILD_TYPE Debug)

include_directories(include)
# include_directories(include)
# Add main.cpp file of project root directory as source file
set(SOURCE_FILES src/main.cpp src/json.cpp)

# Add executable target with source files listed in SOURCE_FILES variable
add_executable(json_lib ${SOURCE_FILES})