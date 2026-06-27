cmake_minimum_required(VERSION 3.20)
project(get-started-cpp LANGUAGES CXX)

set(CMAKE_CXX_STANDARD            23)
set(CMAKE_CXX_STANDARD_REQUIRED   ON)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_executable(
  name_of_exe 
  main.cpp
  src/a.cpp
)

target_include_directories(name_of_exe PRIVATE include)
target_compile_options(name_of_exe PRIVATE -Wall -Wextra)
