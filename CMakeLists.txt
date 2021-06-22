cmake_minimum_required(VERSION 3.16)

project(altair)

set(SOURCE_DIR ${CMAKE_CURRENT_LIST_DIR}/src)
file(GLOB_RECURSE SRC ${SOURCE_DIR}/*.cpp ${SOURCE_DIR}/*.h)

add_executable(altair ${SRC})
target_include_directories(altair PUBLIC ${SOURCE_DIR})