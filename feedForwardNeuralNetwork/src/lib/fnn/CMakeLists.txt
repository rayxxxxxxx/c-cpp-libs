set(src ${CMAKE_SOURCE_DIR}/src)

add_library(FNN SHARED
    ${src}/lib/fnn/fnn.cpp
    ${src}/lib/fnn/dataset.cpp
)

target_link_libraries(FNN PRIVATE
    Linalg
)

target_include_directories(FNN PRIVATE
    ${src}/include
)

