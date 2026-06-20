cmake_minimum_required(VERSION 3.16)
project(BacktestEngine LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
# 开启O2优化，贴近实盘编译习惯
set(CMAKE_CXX_FLAGS_RELEASE "-O2")

file(GLOB SRC src/*.cpp)
add_executable(backtest ${SRC})
