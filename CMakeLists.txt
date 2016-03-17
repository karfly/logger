#cmake_minimum_required(VERSION 3.3)
project(logger)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -lpthread")

set(SOURCE_FILES logger.c ./ring_buffer/ring_buffer.c logger_test.c ret_code.h)
add_executable(logger ${SOURCE_FILES})