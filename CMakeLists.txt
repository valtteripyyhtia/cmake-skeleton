cmake_minimum_required(VERSION 2.8)
set(PROJECT_NAME SkeletonProject)
project(${PROJECT_NAME})

set(CMAKE_CXX_STANDARD 11)

set(PROJECT_VERSION_MAJOR 0)
set(PROJECT_VERSION_MINOR 0)
set(PROJECT_VERSION_PATCH 0)
set(PROJECT_VERSION ${PROJECT_VERSION_MAJOR}.${PROJECT_VERSION_MINOR}.${PROJECT_VERSION_PATCH})

add_subdirectory(src)
add_subdirectory(tests)

enable_testing()
add_test(NAME all_tests COMMAND TestAll)

