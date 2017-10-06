cmake_minimum_required(VERSION 3.6)
project(HelloC)

set(CMAKE_C_STANDARD 90)
set(SOURCE_FILES main.c)


add_executable(HelloC ${SOURCE_FILES})
target_link_libraries(HelloC m)
target_compile_options(HelloC PRIVATE -pedantic -pedantic-errors -Wall -Wextra -Werror)
