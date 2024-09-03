cmake_minimum_required(VERSION 3.29)
project(C___graphics_leaning)

set(CMAKE_CXX_STANDARD 17)

# Find pakages
find_package(glfw3 3.3 REQUIRED)
find_package(OpenGL REQUIRED)
find_package(glad CONFIG REQUIRED)

# Add executable
add_executable(C___graphics_leaning main.cpp)

# Link GLFW, OpenGL, and GLAD
target_link_libraries(C___graphics_leaning glfw OpenGL::GL glad::glad)