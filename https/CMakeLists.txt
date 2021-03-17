cmake_minimum_required(VERSION 3.16)
project(https CXX)

# All samples based on https://quuxplusone.github.io/blog/2020/01/24/openssl-part-1/ tutorial

set (CMAKE_EXPORT_COMPILE_COMMANDS ON)
set (CMAKE_CXX_STANDARD_REQUIRED ON)
set (CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)

add_subdirectory(./client)
add_subdirectory(./server)


