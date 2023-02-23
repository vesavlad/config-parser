cmake_minimum_required(VERSION 3.5)

project(configparser CXX)

file(GLOB_RECURSE cfgparser_SRC src/*.cpp)

add_library(configparser ${cfgparser_SRC})
target_include_directories(configparser PUBLIC ${CMAKE_CURRENT_LIST_DIR}/include)
target_compile_features(configparser PUBLIC cxx_std_11)
