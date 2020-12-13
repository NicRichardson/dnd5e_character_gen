CMAKE_MINIMUM_REQUIRED(VERSION 3.1 FATAL_ERROR)
project(dnd5e_character_gen LANGUAGES CXX)

option(ENABLE_ASAN  "Define ENABLE_ASAN"  FALSE)
option(ENABLE_UBSAN "Define ENABLE_UBSAN" FALSE)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

#find_package(Catch2 REQUIRED)

include_directories(include)

add_executable(character_gen app/character_gen.cpp)

#target_link_libraries(character_gen PUBLIC Catch2::Catch2)
