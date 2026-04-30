cmake_minimum_required(VERSION 3.21)
project(http)

find_package(Boost REQUIRED)

add_executable(myapp src/main.cpp src/utils.cpp)
target_include_directories(myapp PRIVATE 
    include 
    ${Boost_INCLUDE_DIRS}
    )
    