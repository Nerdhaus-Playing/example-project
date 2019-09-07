add_executable(Example_Executable
	main.cpp
)

add_library(Example_Library
	exampleLib.h 
	exampleLib.cpp
)

target_include_directories(Example_Library
	PUBLIC ${CMAKE_CURRENT_LIST_DIR}
)

target_link_libraries(Example_Executable
	Example_Library
)