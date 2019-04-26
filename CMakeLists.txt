# TODO: determine CMAKE_SYSTEM_NAME on OS/390.  Currently assumes "OS/390".
cmake_minimum_required(VERSION 3.0)
project(uvkafka)

add_subdirectory(${PROJECT_SOURCE_DIR}/depends/libuv-1.28.0)


add_subdirectory(${PROJECT_SOURCE_DIR}/src)