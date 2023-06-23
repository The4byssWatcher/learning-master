cmake_minimum_required(VERSION 3.26)

project(learning)

add_executable(learning
    src/main.cpp
)

#Opencv
find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
target_link_libraries( learning ${OpenCV_LIBS} )
