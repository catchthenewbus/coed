cmake_minimum_required(VERSION 3.10.2)

project(coed)

add_subdirectory(glog)

file(GLOB SOURCES "src/*.cpp")
add_executable(coed ${SOURCES})

target_link_libraries(coed glog::glog)
