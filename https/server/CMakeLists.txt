cmake_minimum_required(VERSION 3.16)
project(https_server CXX)

file(GLOB SOURCES
    server.cpp)

add_executable(${PROJECT_NAME} ${SOURCES})
set_property(TARGET ${PROJECT_NAME} PROPERTY CXX_STANDARD 17)
target_link_libraries(${PROJECT_NAME} ssl crypto)
