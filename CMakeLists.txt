cmake_minimum_required(VERSION 3.10)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_EXTENSIONS TRUE)

project(generate_input_helper)

set(SOURCES
    src/models/tscn.h
    src/models/tscn.cpp
    src/main.cpp
)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_SOURCE_DIR}/bin/win/x64")

add_executable(helper ${SOURCES})