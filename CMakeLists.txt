﻿# CMakeList.txt : CMake project for Gameboy Emulator, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

project ("Gameboy Emulator")

# Add source to this project's executable.
add_executable (emu "main.cpp")

target_link_libraries(emu ${CMAKE_CURRENT_SOURCE_DIR}/lib/SDL2.lib)
target_link_libraries(emu ${CMAKE_CURRENT_SOURCE_DIR}/lib/SDL2main.lib)

