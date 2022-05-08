cmake_minimum_required(VERSION 2.8)

project(ScrapyNBA)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_library(libScrapyNBAData SHARED libScrapyNBAData/libScrapyNBAData.cpp)

add_executable(ScrapyNBA main.cpp)

target_link_libraries(ScrapyNBA libScrapyNBAData)

