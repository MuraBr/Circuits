cmake_minimum_required(VERSION 3.29)
project(Circuits)

set(CMAKE_CXX_STANDARD 14)

include_directories(C:\\SFML\\include)
link_directories(C:\\SFML\\lib)

add_executable(Circuits src/main.cpp
        include/ANDGateDrawable.cpp
        include/ComponentDrawable.cpp
        include/App.cpp
        include/ComponentLogic.cpp
        include/DrawableManager.cpp
        include/FileManager.cpp
        include/UIManager.cpp
        include/ANDGateLogic.h
        include/ANDGateLogic.cpp
        include/ANDGateDrawable.h
        include/App.h
        include/ComponentLogic.h
        include/ComponentDrawable.h
        include/DrawableManager.h
        include/FileManager.h
        include/UIManager.h)
target_link_libraries(Circuits -lsfml-system-d -lsfml-window-d -lsfml-graphics-d -lsfml-audio-d)

