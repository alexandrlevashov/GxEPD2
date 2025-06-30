
cmake_minimum_required(VERSION 3.5)

file(GLOB_RECURSE GxEPD_SRC "${CMAKE_CURRENT_LIST_DIR}/*.cpp")

idf_component_register(SRC_DIRS "src" "src/epd"
                       INCLUDE_DIRS "src" "src/bitmaps" "src/epd"
                       REQUIRES Adafruit-GFX-Library)

project(GxEPD2)
