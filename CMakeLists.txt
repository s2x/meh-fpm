cmake_minimum_required(VERSION 3.2)
project(meh-fpm)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES
        mehfpm.cpp
        httpdCodes.h
        preforkServer.cpp
        preforkServer.h
        )

add_executable(meh-fpm ${SOURCE_FILES})