cmake_minimum_required(VERSION 3.12.4)
project(clue CXX)
set(CMAKE_CXX_STANDARD 17)

add_library(${PROJECT_NAME} INTERFACE)
target_include_directories(${PROJECT_NAME} INTERFACE "${CMAKE_CURRENT_SOURCE_DIR}/include/clue")


# function(add_example name)
# add_executable(${name}
#   examples/${name}.cpp
# )
# if(MSVC)
#   target_compile_options(${name} PRIVATE /W4 /WX)
# else()
#   target_compile_options(${name} PRIVATE -Wall -Werror -Wpedantic)
# endif()
# endfunction()
#
# add_example(simple)
# add_example(features)
# add_example(add)
# add_example(vector)
# add_example(user_types)
