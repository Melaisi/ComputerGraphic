
# Set third party path
set(EXTERNAL_DIR "${CMAKE_CURRENT_SOURCE_DIR}" CACHE INTERNAL "")

######### glad #########
# Set GLAD include and src paths
set(GLAD_INCLUDE_DIR "${EXTERNAL_DIR}/glad/include" CACHE INTERNAL "")

set(GLAD_SRC_DIR "${EXTERNAL_DIR}/glad/src" CACHE INTERNAL "")

include_directories(glad/include)

######### glfw #########
# Set GLFW Options
set(GLFW_BUILD_DOCS OFF CACHE BOOL "" FORCE)
set(GLFW_BUILD_TESTS OFF CACHE BOOL "" FORCE)
set(GLFW_BUILD_EXAMPLES OFF CACHE BOOL "" FORCE)

add_subdirectory(glfw-3.4)

# Include glfw
include_directories(
    glfw-3.4/include
)