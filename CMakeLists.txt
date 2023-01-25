cmake_minimum_required(VERSION 3.9) #最低版本

project(helloworld VERSION 1.0) #项目名称及自定义版本号
add_executable(hello_cmake sample_exporter.cpp) #添加生成可执行文件

if(MSVC)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} /std:c++17")
endif(MSVC)