# CMakeList.txt: проект CMake для test; включите исходный код и определения,
# укажите здесь логику для конкретного проекта.
#
cmake_minimum_required (VERSION 3.8)

project ("test")

# Добавьте источник в исполняемый файл этого проекта.
add_executable (test "test.cpp" "test.h")

# TODO: Добавьте тесты и целевые объекты, если это необходимо.


if(NOT CMAKE_BUILD_TYPE)
  set(CMAKE_BUILD_TYPE Release)
endif()

IF (CMAKE_COMPILER_IS_GNUCXX)
set(CMAKE_CXX_FLAGS "-Wall -std=c++11")
ENDIF (CMAKE_COMPILER_IS_GNUCXX)
