cmake_minimum_required(VERSION 3.30.0)

project(learn_vulkan LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

file(GLOB_RECURSE SOURCES "src/*.cpp")
file(GLOB_RECURSE HEADERS "src/*.h")

add_executable(learn_vulkan ${SOURCES} ${HEADERS})

