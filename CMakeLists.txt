cmake_minimum_required(VERSION 3.29)
project(Tests)

set(CMAKE_CXX_STANDARD 20)
set(GCC_COVERAGE_COMPILE_FLAGS "-Wall -Werror -Wextra -fsanitize=address,undefined ")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${GCC_COVERAGE_COMPILE_FLAGS}" )

add_executable(differential_task
        differential_base.cpp)
