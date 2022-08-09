cmake_minimum_required(VERSION 3.2)
project(template_project)

add_subdirectory(feature)
set(SOURCE_FILES main.cpp)

add_executable(template_project ${SOURCE_FILES})
target_link_libraries(template_project feature)
install(TARGETS template_project DESTINATION ${DIVISIBLE_INSTALL_BIN_DIR})
