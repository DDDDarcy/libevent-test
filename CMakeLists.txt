cmake_minimum_required(VERSION 3.2)

project(MyProject)

#set(LIST_SRC ./test-src)

include_directories(./test-include)
aux_source_directory(./test-src LIST_SRC)

add_executable(my_app main.cpp)
link_directories(LIST_SRC)