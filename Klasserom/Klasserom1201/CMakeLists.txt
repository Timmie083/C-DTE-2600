cmake_minimum_required(VERSION 3.5)

project(Klasserom1201 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(Klasserom1201 main.cpp
    testfredag.h testfredag.cpp)

include(GNUInstallDirs)
install(TARGETS Klasserom1201
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
