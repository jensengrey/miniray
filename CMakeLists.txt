cmake_minimum_required(VERSION 2.8.12)
project(miniray)

set(GCC_COVERAGE_COMPILE_FLAGS "-g3 -fno-omit-frame-pointer -fno-inline")

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${GCC_COVERAGE_COMPILE_FLAGS}")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${GCC_COVERAGE_COMPILE_FLAGS}")


set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR})

add_subdirectory(src)


