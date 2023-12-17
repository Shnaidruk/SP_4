cmake_minimum_required(VERSION 3.10)
project(Calculatoras)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES main.cpp calculator.cpp calculator.h)

add_library(calculator STATIC ${SOURCE_FILES})

add_executable(calculatoras main.cpp)
target_link_libraries(calculatoras calculator)