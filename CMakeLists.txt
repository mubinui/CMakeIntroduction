cmake_minimum_required(VERSION 3.24)
project(Introduction)

set(CMAKE_CXX_STANDARD 20)

add_subdirectory(include)
add_subdirectory(src)
option(BUILD_EXAMAPLES "Whether of not to build examples" ON)
if (BUILD_EXAMPLES)
    message(STATUS "Building Example")
    add_subdirectory(example)
endif()


