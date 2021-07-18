cmake_minimum_required(VERSION 2.8.12)
project(encrypted_fileserver)

add_definitions("-std=c++11")

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

add_executable(encrypted_fileserver encrypted_fileserver.cpp)
target_link_libraries(encrypted_fileserver ${CONAN_LIBS})

