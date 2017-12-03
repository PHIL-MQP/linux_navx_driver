cmake_minimum_required (VERSION 2.8)
project (linux_navx_driver)
add_definitions(-std=c++11 -Wall -Wextra -Wno-switch)

file(GLOB SOURCES
	"*.h"
	"*.cpp"
)

include_directories(".")
add_library(NavXTimeStamp ${SOURCES})

