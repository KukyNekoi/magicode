cmake_minimum_required(VERSION 3.16)
project(iqs_test)

set(CMAKE_CXX_STANDARD 14)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS}")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS}")


set(PROJECT_HEADERS
        src/IQS.h
        src/BareBoneIQS.h
        src/IIQS.h
        src/rIIQS.h
        src/BareBoneIIQS.h flags.h)
set(PROJECT_SOURCES
        main.cpp
        src/IQS.cpp
        src/BareBoneIQS.cpp
        src/IIQS.cpp
        src/rIIQS.cpp
        src/BareBoneIIQS.cpp)

add_executable(iqs_test ${PROJECT_SOURCES} ${PROJECT_HEADERS})