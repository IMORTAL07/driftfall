cmake_minimum_required(VERSION 3.20)

project(Driftfall LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_subdirectory(engine)

add_executable(driftfall
    src/main.cpp
)

target_link_libraries(driftfall
    PRIVATE axiom
)
