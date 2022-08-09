cmake_minimum_required(VERSION 3.2)
project(feature C CXX)

set(SOURCE_FILES
    feature.h
    feature.cpp
)

add_library(feature SHARED STATIC ${SOURCE_FILES})

install(TARGETS feature DESTINATION ${DIVISIBLE_INSTALL_LIB_DIR})
install(FILES feature.h DESTINATION ${DIVISIBLE_INSTALL_INCLUDE_DIR})
