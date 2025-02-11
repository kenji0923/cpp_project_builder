cmake_minimum_required(VERSION 3.5 FATAL_ERROR)


project(VAR_PROJECT_NAME)


set(CMAKE_CXX_STANDARD 17)


option(BUILD_SHARED_LIBS "Build using shared libraries" OFF)


if(NOT CMAKE_BUILD_TYPE)
    set(CMAKE_BUILD_TYPE Release)
endif()
set(CMAKE_CXX_FLAGS_RELEASE "-Ofast")


add_subdirectory(${PROJECT_SOURCE_DIR}/document)
add_subdirectory(${PROJECT_SOURCE_DIR}/core)
