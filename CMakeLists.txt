cmake_minimum_required(VERSION 3.1)
project(write_test)

set(CMAKE_CXX_STANDARD 11)
find_package(OpenCV REQUIRED)
add_executable(write_test main.cpp
        ${OpenCV_INCLUDE_DIRS}
        )

target_link_libraries(write_test
        ${OpenCV_LIBRARIES}
        )
