cmake_minimum_required(VERSION 3.25.0)
project(CppDrawingWithD2dKerr VERSION 1.0)

# Specify the C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

add_definitions(
    /D_UNICODE=1
    /DUNICODE=1
)

include_directories("./wtl")

set(MY_EXECUTABLE_NAME "CppDrawingWithD2dKerr")
set(
  SOURCE_FILES
  "./src/main.cpp"
)

add_executable(${MY_EXECUTABLE_NAME} WIN32 ${SOURCE_FILES})
