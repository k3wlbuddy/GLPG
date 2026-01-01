set(GLPG_INCLUDES PRIVATE ${CMAKE_SOURCE_DIR}/include ${CMAKE_SOURCE_DIR}/sdk/d3d8/include)

set(GLPG_SOURCES)

add_executable(01_clear_color_d3d8 01_clear_color.cpp)

target_include_directories(01_clear_color_d3d8 ${GLPG_INCLUDES})
target_link_libraries(01_clear_color_d3d8 glpg)
target_compile_features(01_clear_color_d3d8 PUBLIC cxx_std_17)

add_executable(02_hello_triangle_d3d8 02_hello_triangle.cpp)

target_include_directories(02_hello_triangle_d3d8 ${GLPG_INCLUDES})
target_link_libraries(02_hello_triangle_d3d8 glpg)
target_compile_features(02_hello_triangle_d3d8 PUBLIC cxx_std_17)
