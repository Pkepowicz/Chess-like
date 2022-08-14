# CMakeList.txt : CMake project for Chess-like, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

project ("Chess-like")

# Add source to this project's executable.
add_executable (Chess-like "main.cpp" "Board.cpp" "Board.h")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET Chess-like PROPERTY CXX_STANDARD 20)
endif()

# TODO: Add tests and install targets if needed.
