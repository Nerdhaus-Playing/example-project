cmake_minimum_required(VERSION 3.12)

project(Example VERSION 1.0.0
                  DESCRIPTION "Example Project to show and test different technologies like Cmake, conan, CPack"
                  LANGUAGES CXX)

set_property(GLOBAL PROPERTY USE_FOLDERS ON)



set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)
set(CMAKE_EXECUTABLE_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)

add_subdirectory(src)
