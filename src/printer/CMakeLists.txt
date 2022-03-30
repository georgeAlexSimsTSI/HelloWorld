add_library(
    printer
    printer.h
    printer.cpp
)

target_include_directories(printer PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/src")