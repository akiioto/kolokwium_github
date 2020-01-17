cmake_minimum_required(VERSION 3.10)
project(dynamiclib)

file(GLOB SOURCES src/*.cpp)

include_directories(include)

add_library(${PROJECT_NAME} SHARED ${SOURCES})

install(TARGETS ${PROJECT_NAME} DESTINATION lib/${PROJECT_NAME})

file(GLOB HEADERS include/*.h)
install(FILES ${HEADERS} DESTINATION include/${PROJECT_NAME})
