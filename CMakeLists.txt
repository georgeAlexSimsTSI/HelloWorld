
cmake_minimum_required(VERSION 3.10)

set(CMAKE_CXX_STANDARD 20)

set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(HelloWorld VERSION 2.0)


add_library(
    printer
    src/printer.h
    src/printer.cpp
)

add_executable(${PROJECT_NAME} src/main.cpp)

target_link_libraries(${PROJECT_NAME} PRIVATE printer)

target_compile_features(${PROJECT_NAME} PUBLIC cxx_std_20)


