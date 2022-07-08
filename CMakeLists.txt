cmake_minimum_required(VERSION 3.10)

project(sandwich_cSEM Fortran)

enable_language(Fortran C)

# set(CMAKE_Fortran_FLAGS "${CMAKE_Fortran_FLAGS} -ffree-line-length -O3")

# find_package(MPI REQUIRED)

find_package(MPI REQUIRED)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_Fortran_MODULE_DIRECTORY ${CMAKE_BINARY_DIR}/mod)

include_directories(${CMAKE_Fortran_MODULE_DIRECTORY})

add_subdirectory(yannos)
add_subdirectory(nms)
add_subdirectory(stock_boule)


