cmake_minimum_required(VERSION 3.30)
project(space_invaders C)

set(CMAKE_C_STANDARD 11)

find_package(SDL3 REQUIRED COMPONENTS SDL3)
add_executable(space_invaders main.c)
target_link_libraries(space_invaders PRIVATE SDL3::SDL3)