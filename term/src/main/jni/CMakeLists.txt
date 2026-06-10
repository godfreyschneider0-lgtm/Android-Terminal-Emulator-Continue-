cmake_minimum_required(VERSION 3.10.2)

project("jackpal-androidterm5")

add_library(
    jackpal-androidterm5
    SHARED
    common.cpp
    fileCompat.cpp
    termExec.cpp
)

find_library(
    log-lib
    log
)

target_link_libraries(
    jackpal-androidterm5
    ${log-lib}
)
