cmake_minimum_required(VERSION 3.4.1)

PROJECT (HELLO)
SET(SRC_LIST main.c)
MESSAGE(STATUS "This is BINARY dir " ${PROJECT_BINARY_DIR})
MESSAGE(STATUS "This is SOURCE dir " ${PROJECT_SOURCE_DIR})
ADD_EXECUTABLE(hello ${SRC_LIST})
