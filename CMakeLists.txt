cmake_minimum_required(VERSION 3.10)
project(TonyCppApp)

add_library(main SHARED main.cpp)

find_library(log-lib log)
target_link_libraries(main ${log-lib} android SDL2)
