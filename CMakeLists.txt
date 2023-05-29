cmake_minimum_required(VERSION 3.0)
project(open62541_server C)

add_executable(${PROJECT_NAME} src/main.c)

find_package(open62541)

target_link_libraries(${PROJECT_NAME} open62541)
