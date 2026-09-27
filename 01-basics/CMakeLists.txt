cmake_minimum_required(VERSION 3.10)

# Name your project
project(MyApp)

# Set the C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Create the executable from the source files
add_executable(my_app src/main.cpp src/math_utils.cpp)

# Tell the compiler where to find the header files
target_include_directories(my_app PRIVATE ${CMAKE_SOURCE_DIR}/include)