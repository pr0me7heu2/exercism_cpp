cmake_minimum_required(VERSION 3.13)
project(cpp)

set(CMAKE_CXX_STANDARD 14)

include_directories(hello-world)
include_directories(hello-world/test)

add_executable(cpp
        hello-world/test/catch.hpp
        hello-world/test/tests-main.cpp
        hello-world/CMakeLists.txt
        hello-world/hello_world.cpp
        hello-world/hello_world.h
        hello-world/hello_world_test.cpp)
