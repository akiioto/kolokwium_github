cmake_minimum_required(VERSION 3.10)
# set the project name
project(myProgram)
file(GLOB SOURCES "src/*.cpp")
include_directories(include)

# add the executable
add_executable(myProgram ${SOURCES})

