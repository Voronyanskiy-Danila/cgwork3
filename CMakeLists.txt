cmake_minimum_required(VERSION 3.16)
project(SoftwareRenderer LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

set(SRC_FILES
    src/main.cpp
    src/image.cpp
    src/model.cpp
    src/rasterizer.cpp
    src/shader.cpp
)

add_executable(software_renderer ${SRC_FILES})
target_include_directories(software_renderer PRIVATE include)
