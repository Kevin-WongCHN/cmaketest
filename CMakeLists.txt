# 最低CMake版本要求
cmake_minimum_required(VERSION 3.10)

# 项目信息
project(MyProject)
include_directories(inc)
add_executable(calculator src/calculator.c src/test_calculator.c)
enable_testing()
add_test(NAME MyTest COMMAND calculator)