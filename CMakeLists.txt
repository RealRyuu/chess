cmake_minimum_required(VERSION 2.8.12)
project(Chess)

set(CMAKE_CXX_STANDARD 20)

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

add_executable(Chess source/main.cpp)
target_link_libraries(Chess ${CONAN_LIBS})