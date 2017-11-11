cmake_minimum_required(VERSION 3.8)
project(TutorialTwo)

set(CMAKE_CXX_STANDARD 11)

link_libraries(SDL2)

set(SOURCE_FILES TutorialTwo/*.cpp)
add_executable(TutorialTwo ${SOURCE_FILES})