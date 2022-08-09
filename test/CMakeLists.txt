cmake_minimum_required(VERSION 3.2)
project(template_project_tests)

add_subdirectory(lib/googletest)

include_directories(${DIVISION_HEADERS_DIR})
include_directories(lib/googletest/googletest/include)

set(SOURCE_FILES main.cpp src/template_project_tests.cpp)

add_executable(template_project_tests ${SOURCE_FILES})
target_link_libraries(template_project_tests feature gtest)
install(TARGETS template_project_tests DESTINATION bin)

