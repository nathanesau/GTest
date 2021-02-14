cmake_minimum_required(VERSION 3.10)

project(stats)

add_subdirectory(src)

if (UNIX)
    enable_testing()
    add_subdirectory(test)
endif (UNIX)