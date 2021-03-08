 cmake_minimum_required(VERSION 2.8.12)
 project(Hydrogen)

 add_definitions("-std=c++11")

 include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
 conan_basic_setup()

 add_executable(hydrogen main.cpp main.cpp)
 target_link_libraries(hydrogen ${CONAN_LIBS})
