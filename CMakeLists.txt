project(optional)
cmake_minimum_required(VERSION 2.8)
enable_testing()

set(CMAKE_CXX_FLAGS "-std=c++0x -Wall -Wextra -Wold-style-cast -Winit-self -Werror=return-type -pedantic")

add_executable(test_optional test_optional.cpp)
add_executable(test_type_traits test_type_traits.cpp)

add_test(test_optional test_optional)
add_test(test_type_traits test_type_traits)
