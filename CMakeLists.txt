cmake_minimum_required(VERSION 2.8.4)
set(CMAKE_TOOLCHAIN_FILE ${CMAKE_SOURCE_DIR}/cmake/ArduinoToolchain.cmake)
set(PROJECT_NAME PGA2311-VFD)
project(${PROJECT_NAME})

set(${CMAKE_PROJECT_NAME}_SKETCH PGA2311-VFD.ino)
generate_arduino_firmware(${CMAKE_PROJECT_NAME})
set(${FIRMWARE_NAME}_PORT "\\\\\.\\COM5")