cmake_minimum_required(VERSION 3.5)

project(Library LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(Library main.cpp book.h book.cpp reader.h reader.cpp copy.h copy.cpp)

install(TARGETS Library
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR})
