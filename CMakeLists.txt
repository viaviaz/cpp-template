cmake_minimum_required(VERSION 3.0.0)
project(samplate-cpp-template VERSION 0.1.0)

include(CTest)
enable_testing()
include_directories(./include)
aux_source_directory(./src DIR_SRCS)
add_executable(samplate-cpp-template ${DIR_SRCS} main.cpp )

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
