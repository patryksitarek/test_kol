cmake_minimum_required(VERSION 3.13.4)
project(directory_test)

include_directories(include)

file(GLOB SOURCES "src/*.cpp")

add_executable(myProgram ${SOURCES})
