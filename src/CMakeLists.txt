ADD_EXECUTABLE(hellocmake test.cpp)

if(ENABLE_MPI)
	target_link_libraries(hellocmake ${MPI_LIBRARIES})
endif(ENABLE_MPI)


