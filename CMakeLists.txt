
cmake_minimum_required(VERSION 3.10)

set(CMAKE_CXX_STANDARD 20)

set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(HelloWorld VERSION 2.0)

add_subdirectory(src/printer) #Libraries first
add_subdirectory(src/main)
