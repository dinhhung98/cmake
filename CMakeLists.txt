cmake_minimum_required(VERSION 2.8.12)
project (cmake8)
include_directories(include)
set(SOURCES main/fn.c)
add_library(funny STATIC ${SOURCES})
add_executable(funny_app main/main.c)
target_link_libraries(funny_app funny)
