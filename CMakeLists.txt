cmake_minimum_required(VERSION 3.1.0)

project(App_launcher)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

find_package(Qt5 COMPONENTS Widgets REQUIRED)

add_executable(${PROJECT_NAME}
    src/mainwindow.ui
    src/mainwindow.cpp
    src/main.cpp
)

target_link_libraries(${PROJECT_NAME} Qt5::Widgets)

