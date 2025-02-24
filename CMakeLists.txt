cmake_minimum_required(VERSION 3.6)
project(openmp_test_clion)

# added -fopenmp
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -fopenmp")

add_executable(executable1 generate.cpp)
add_executable(executable2 serial.cpp)
add_executable(executable3 cpu-parallel.cpp)