cmake_minimum_required(VERSION 3.16.3)

set(MAKE_CXX_COMPILER /usr/bin/g++)
set(MAKE_C_COMPILER /usr/bin/gcc)

project(MyProject)

add_library(MyProdlib STATIC 
	main.c 
	my_lib.c 
	my_lib.h
)

add_executable(
	MyProject
	./main.c
	./my_lib.c	
)
