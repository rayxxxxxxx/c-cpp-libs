cmake_minimum_required(VERSION 3.2)

project(CSVReader)

add_subdirectory(${CMAKE_SOURCE_DIR}/src/lib)

add_executable(app ${CMAKE_SOURCE_DIR}/src/main.cpp)

target_link_libraries(app PRIVATE CSVReader)
