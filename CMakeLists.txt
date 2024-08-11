cmake_minimum_required(VERSION 3.28.0)

project(OpenGLSandbox VERSION 1.0.0)

# Add openGL
find_package(OpenGL REQUIRED)
include_directories(${OPENGL_INCLUDE_DIR})

# Add and set external Dependencies
add_subdirectory(external)

# add targets from source code folder
add_subdirectory(src)