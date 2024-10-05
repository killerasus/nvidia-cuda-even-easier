cmake_minimum_required(VERSION 3.28)

project(EvenEasierIntroductionToCUDA 
        DESCRIPTION "Examples of the NVIDIA course An Even Easier Introduction to CUDA."
        LANGUAGES CUDA CXX
)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_subdirectory(src/cpu)
add_subdirectory(src/gpu)