cmake_minimum_required(VERSION 3.14)

project(CalculatorProject)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_subdirectory(googletest)

add_executable(calculator_test
    calculator.cpp
    calculator_test.cpp
)

target_link_libraries(calculator_test
    GTest::gtest_main
)