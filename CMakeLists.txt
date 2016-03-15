cmake_minimum_required(VERSION 3.3)
project(logger)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -lpthred")

set(SOURCE_FILES logger.c ./ring_buffer/ring_buffer.c)
add_executable(logger ${SOURCE_FILES})