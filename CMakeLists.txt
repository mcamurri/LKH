cmake_minimum_required(VERSION 2.8.3)
project(lkh_tsp_solver)

set(CMAKE_BUILD_TYPE "Release")

include_directories(SRC/INCLUDE)

file(GLOB SRCS SRC/*.c )

add_executable(lkh_tsp ${SRCS})
target_link_libraries(lkh_tsp -lm)

#add_executable(lkh_tsp SRC/LKHmain.c)
#target_link_libraries(lkh_tsp lkh_tsp_solver)
