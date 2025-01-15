cmake_minimum_required(VERSION 3.30)
project(MarioDeFII)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_MODULE_PATH ${CMAKE_SOURCE_DIR}/cmake_modules)

add_executable(MarioDeFII main.cpp Map.cpp Map.h Enemies.cpp Enemies.h Colectibles.cpp Colectibles.h
        Colissions.cpp Colissions.h Mario.cpp Mario.h Loader.cpp Loader.h Menus.cpp Menus.h MapEditor.cpp
        MapEditor.h Game.cpp Game.h Sounds.cpp Sounds.h miniaudio.h)

target_link_libraries(MarioDeFII
        -lbgi
        -lgdi32
        -lcomdlg32
        -luuid
        -loleaut32
        -lole32
)
