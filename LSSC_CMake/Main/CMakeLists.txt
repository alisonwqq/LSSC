CMAKE_MINIMUM_REQUIRED(VERSION 2.6)

PROJECT(Main)

SET(SRC main.cpp params.h)

ADD_EXECUTABLE(Main ${SRC})

INCLUDE_DIRECTORIES(..)

TARGET_LINK_LIBRARIES(Main Images IO LSSC ORMP)

INSTALL(FILES CMakeLists.txt ${SRC} DESTINATION src/Main)
