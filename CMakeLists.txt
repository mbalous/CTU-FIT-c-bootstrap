cmake_minimum_required(VERSION 3.6)
project(HelloC)

set(CMAKE_CXX_STANDARD 11)
set(SOURCE_FILES main.c)

add_executable(HelloC ${SOURCE_FILES})
target_link_libraries(HelloC m)
target_compile_options(HelloC PRIVATE -pedantic -Wall -Wextra -g -O2)
