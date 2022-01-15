# Available variables found in OpenCVConfig.cmake
# OpenCV_DIR, OpenCV_VERSION, OpenCV_INCLUDE_DIRS

cmake_minimum_required(VERSION 3.21)
set(CMAKE_CXX_STANDARD 11)
project(first_program)
set(OpenCV_DIR "/usr/local/Cellar/opencv/4.5.4_3")
find_package(OpenCV REQUIRED)
add_executable(headpose headpose.cpp)
target_link_libraries(headpose ${OpenCV_LIBS})
