cmake_minimum_required(VERSION 3.15)
project(Clipper2 VERSION 1.2.2 LANGUAGES C CXX)

set(CMAKE_POSITION_INDEPENDENT_CODE ON)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)
set_property(GLOBAL PROPERTY USE_FOLDERS ON)

option(CLIPPER2_UTILS "Build utilities" ON)
option(CLIPPER2_EXAMPLES "Build examples" ON)
option(CLIPPER2_TESTS "Build tests" ON)
option(USE_EXTERNAL_GTEST "Use system-wide installed GoogleTest" OFF)
option(USE_EXTERNAL_GBENCHMARK "Use the googlebenchmark" OFF) 
option(BUILD_SHARED_LIBS "Build shared libs" OFF)
set(CLIPPER2_USINGZ "ON" CACHE STRING "Build Clipper2Z, either \"ON\" or \"OFF\" or \"ONLY\"")

add_subdirectory(CPP)
