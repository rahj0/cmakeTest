# Specify the library sources
set(LIBRARY_SOURCES MyLibrary.cpp)

# Define the shared library target
add_library(MyLibrary SHARED ${LIBRARY_SOURCES})

# Specify the include directory for the library
target_include_directories(MyLibrary PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

# Set version properties for the library
set_target_properties(MyLibrary PROPERTIES VERSION 1.0 SOVERSION 1)
