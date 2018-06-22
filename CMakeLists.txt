cmake_minimum_required(VERSION 3.9)
project(study)
add_executable(study main.cpp)

set(CMAKE_CXX_STANDARD 11)

find_package(OpenGL REQUIRED)
find_package(GLUT REQUIRED)

include_directories( ${OPENGL_INCLUDE_DIRS}  ${GLUT_INCLUDE_DIRS} )
target_link_libraries(study ${OPENGL_LIBRARIES} ${GLUT_LIBRARY} )


