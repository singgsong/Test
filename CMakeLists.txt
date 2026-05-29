# 声明 CMake 的最低版本要求
cmake_minimum_required(VERSION 3.10)

# 项目名称
project(MyTestProject)

# 指定 C++ 标准（比如 C++17）
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# 寻找源文件并生成可执行文件
# 假设你的主程序叫 main.cpp，生成的可执行文件叫 MyProgram
add_executable(MyProgram main.cpp)

enable_testing()
add_test(NAME RunMyProgram COMMAND MyProgram)
