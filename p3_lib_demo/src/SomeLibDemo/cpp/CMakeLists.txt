cmake_minimum_required(VERSION 3.22.1)
project(bpxmath)
add_library(bpxmath adder.cpp)
set_target_properties(bpxmath PROPERTIES PUBLIC_HEADER adder.h)
install(TARGETS bpxmath LIBRARY DESTINATION lib
	PUBLIC_HEADER DESTINATION include
	)
