﻿# CMakeList.txt : CMake project for raytracer, include source and define
# project specific logic here.
#

# Add source to this project's executable.
add_executable (raytracer "raytracer.cpp" "raytracer.h")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET raytracer PROPERTY CXX_STANDARD 20)
endif()

# TODO: Add tests and install targets if needed.

install (TARGETS raytracer DESTINATION "raytracer/bin")