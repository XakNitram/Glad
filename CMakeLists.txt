cmake_minimum_required(VERSION 3.5)
project(Glad VERSION 0.1.36 LANGUAGES C)

add_library(
    glad
    include/glad/glad.h
    include/KHR/khrplatform.h
    src/glad.c
)

target_include_directories(glad PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/include")
