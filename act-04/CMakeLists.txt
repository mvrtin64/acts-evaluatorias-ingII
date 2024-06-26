cmake_minimum_required(VERSION 3.17)
project(TutCMake2)

set(CMAKE_CXX_STANDARD 11)

add_executable(TutCMake2 main.cpp)

target_compile_features(TutCMake2
    PUBLIC
        cxx_nullptr
    PRIVATE
        cxx_lambdas
)
 
target_compile_options(TutCMake2 PRIVATE -Werror)