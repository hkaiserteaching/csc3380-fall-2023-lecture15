cmake_minimum_required(VERSION 3.19)
project(fall2023-csc3380-lecture15)

set(CMAKE_CXX_STANDARD 20)

add_executable(test_singleton code/test_singleton.cpp)
add_executable(test_instrumented_unique 
    code/test_instrumented_unique.cpp 
    code/instrumented.cpp)
