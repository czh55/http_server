project(http)

cmake_minimum_required(VERSION 3.2.0)

if(NOT TARGET_ARCH)
    set(TARGET_ARCH "native")
endif()
message(STATUS "Build for target architecture: ${TARGET_ARCH}")

add_subdirectory(httpclient)
add_subdirectory(httpserver)
