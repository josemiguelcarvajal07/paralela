cmake_minimum_required(VERSION 2.8)
project(testing)
find_package(OpenCV REQUIRED)
include_directories( ${OpenCV_INCLUDE_DIRS} )
include_directories(/content/paralela/Tests)
add_executable(reduccion1080 /content/paralela/Tests/reduccion1080.cpp)
target_link_libraries(reduccion1080 ${OpenCV_LIBS})