cmake_minimum_required(VERSION 3.13)
project(fast_queue)

set(CMAKE_CXX_STANDARD 17)

add_library(fast_queue SHARED faster_fifo.cpp faster_fifo.hpp)
target_include_directories(fast_queue INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})

add_subdirectory(googletest)
