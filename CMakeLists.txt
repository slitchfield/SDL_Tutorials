cmake_minimum_required(VERSION 3.8)
project(TutorialOne)

set(CMAKE_CXX_STANDARD 11)

link_libraries(SDL2)

set(SOURCE_FILES TutorialOne/01_hello_SDL.cpp)
add_executable(01_hello_SDL ${SOURCE_FILES})