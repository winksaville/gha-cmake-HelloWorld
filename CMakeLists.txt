message(STATUS "first line")
cmake_minimum_required(VERSION 3.16)

message(STATUS "before project")
project(main)

message(STATUS "before add_executable")
add_executable(main main.cpp)

message(STATUS "before install")
install(TARGETS main)

message(STATUS "before enable testing")
enable_testing()

message(STATUS "before add_test")
add_test(NAME main COMMAND main)

message(STATUS "last line")
