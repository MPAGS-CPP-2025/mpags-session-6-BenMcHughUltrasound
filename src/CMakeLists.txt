cmake_minimum_required(VERSION 3.8)
project(MPAGSCipher VERSION 0.1.0)

set(CMAKE_VERBOSE_MAKEFILE ON)
add_executable(mpags-cipher mpags-cipher.cpp
MPAGSCipher/TransformChar.cpp
MPAGSCipher/TransformChar.hpp
MPAGSCipher/ProcessCommandLine.cpp
MPAGSCipher/ProcessCommandLine.hpp)
set(CMAKE_CXX_EXTENSIONS OFF)
set(CMAKE_CXX_FLAGS "-Wall -Wextra -Werror -Wfatal-errors -Wshadow -pedantic")
target_include_directories(mpags-cipher PRIVATE MPAGSCipher)
target_compile_features(mpags-cipher PRIVATE cxx_std_17)