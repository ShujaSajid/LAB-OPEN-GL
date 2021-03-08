cmake_minimum_required(VERSION 3.0.0)
project(LabOpenGL VERSION 0.1.0)

include(CTest)
enable_testing()

set (CMAKE_CXX_FLAGS "-lglfw -lGL -lGLU -lglut -lX11 -lpthread -lXrandr -lXi -ldl")

add_executable(LabOpenGL #main.cpp
                         #chess.cpp
                         triangle.cpp   
                         glad/glad.c)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
