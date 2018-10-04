cmake_minimum_required(VERSION 3.0)

PROJECT (hellocmake)

option(ENABLE_MPI "Enable MPI parallelization" OFF)

if(ENABLE_MPI)
	find_package(MPI REQUIRED)
	include_directories(${MPI_INCLUDE_PATH})
	set(CMAKE_C_FLAGS "${CMAKE_FLAGS} ${MPI_FLAGS}")
	set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${MPI_CXX_FLAGS}")
	set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} ${MPI_EXE_LINKER_FLAGS}")
endif(ENABLE_MPI)

ADD_SUBDIRECTORY (src)
