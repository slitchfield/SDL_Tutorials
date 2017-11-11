cmake_minimum_required(VERSION 3.8)

set(prj_name TutorialTwo)
project(${prj_name})

set(CMAKE_CXX_STANDARD 11)

link_libraries(SDL2)

set(SOURCE_FILES ${prj_name}/02_getting_an_image_on_the_screen.cpp)
add_executable(${prj_name} ${SOURCE_FILES})


add_custom_command(TARGET ${prj_name} POST_BUILD
        COMMAND cp ./${prj_name} ../${prj_name}/${prj_name}
        )