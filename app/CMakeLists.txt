# Specify the executable
add_executable(MyApp main.cpp)

# Link the executable to the library
target_link_libraries(MyApp PRIVATE MyLibrary)

set_target_properties(MyApp PROPERTIES LINK_DEPENDS_NO_SHARED true)