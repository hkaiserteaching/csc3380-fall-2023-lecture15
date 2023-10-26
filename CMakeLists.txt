cmake_minimum_required(VERSION 3.19)
project(fall2023-csc3380-lecture15)

set(CMAKE_CXX_STANDARD 20)

find_package(FLTK CONFIG REQUIRED)

set(fltk_toolkit_sources
    code/Graph.cpp
    code/GUI.cpp
    code/Simple_window.cpp
    code/Window.cpp
)

add_executable(display_model code/display_model.cpp ${fltk_toolkit_sources})
target_link_libraries(display_model PRIVATE fltk fltk_images)

add_executable(demo code/demo.cpp ${fltk_toolkit_sources})
target_link_libraries(demo PRIVATE fltk fltk_images)
