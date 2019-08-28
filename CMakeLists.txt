cmake_minimum_required(VERSION 3.11)
project(open-dis-cpp)


FILE(GLOB DIS6_SRC src/dis6/*.cpp )
FILE(GLOB DIS6_HDR src/dis6/*.h )
FILE(GLOB UTILS_SRC src/utils/*.cpp)
FILE(GLOB UTILS_HDR src/utils/*.h)

add_library(OpenDIS ${DIS6_SRC} ${DIS6_HDR} ${UTILS_SRC} ${UTILS_HDR})
target_include_directories(OpenDIS PRIVATE src)

