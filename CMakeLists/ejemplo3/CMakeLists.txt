cmake_minimum_required(VERSION 3.10)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

project(App LANGUAGES CXX)

set(SRC_DIR ${PROJECT_SOURCE_DIR}/src)
set(SRC_LST ${SRC_DIR}/main.cpp)
set(INC_DIR ${PROJECT_SOURCE_DIR}/include)

add_executable(${PROJECT_NAME} ${SRC_LST})

target_include_directories(${PROJECT_NAME} PUBLIC ${INCLUDE_DIR})
