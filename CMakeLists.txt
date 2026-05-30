cmake_minimum_required(VERSION 3.10)

project(main C)

add_executable(main)

target_include_directories(main PRIVATE my_lib)

target_sources(main
    PRIVATE
    hello.c
    my_lib/hellofunc.c
)
