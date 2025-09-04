cmake_minimum_required(VERSION 3.30)
project(GTest_UnitTests)

set(GTest_SOURCE_DIR "${CMAKE_SOURCE_DIR}/googletest-src" CACHE PATH "Path to googletest source")

# If not already added, add it
if(NOT TARGET gtest)
    add_subdirectory(${GTest_SOURCE_DIR} ${CMAKE_BINARY_DIR}/googletest-build)
endif()
