project(helloWorld)

message("${GLAD_SRC_DIR}")
message("-----------------------")

add_executable(helloWorldOut main.cpp "${GLAD_SRC_DIR}/glad.c")

target_link_libraries(helloWorldOut ${OPENGL_LIBRARY} glfw )
include_directories(${GLAD_INCLUDE_DIR})