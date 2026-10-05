cmake_minimum_required(VERSION 3.16)

project(MyQtApp LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_PREFIX_PATH "C:/Qt/6.12.0/msvc2022_64")

find_package(Qt6 REQUIRED COMPONENTS Widgets)

qt_standard_project_setup()

qt_add_executable(MyQtApp
    main.cpp
)

target_link_libraries(MyQtApp PRIVATE Qt6::Widgets)
