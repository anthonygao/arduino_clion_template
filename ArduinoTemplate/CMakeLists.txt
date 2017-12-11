cmake_minimum_required(VERSION 3.9)
project(ArduinoTemplate)

set(CMAKE_CXX_STANDARD 11)

# include Ardunio headers for interception
include_directories(../arduino/cores ../arduino/tools)
include_directories(../arduino/variants/mega)

# include Ardunio libraries
include_directories(../arduino/libraries/Wire/src)
include_directories(../arduino/libraries/SPI/src)
include_directories(../arduino/libraries/SoftwareSerial/src)
include_directories(../arduino/libraries/HID/src)
include_directories(../arduino/libraries/EFPROM/src)


# include custom libraries

add_executable(ArduinoTemplate main.cpp)