cmake_minimum_required(VERSION 3.27)
project(lunarweb)

set(CMAKE_CXX_STANDARD 20)

add_subdirectory(luajit-cmake)
target_link_libraries(yourTarget PRIVATE luajit::lib luajit::header)

add_executable(lunarweb main.cpp)
