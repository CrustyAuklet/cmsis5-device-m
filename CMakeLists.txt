cmake_minimum_required(VERSION 3.15)
project(CMSIS
        VERSION 5.4.0
        DESCRIPTION "CMSIS 5 Core as a CMake package"
        LANGUAGES C ASM)

add_library(CMSIS_CORE INTERFACE)
add_library(CMSIS::CORE ALIAS CMSIS_CORE)

target_include_directories(CMSIS_CORE INTERFACE ${CMAKE_CURRENT_LIST_DIR}/Core/Include)
