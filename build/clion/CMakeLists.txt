cmake_minimum_required(VERSION 3.8)
project(cfminimal)

set(CMAKE_CXX_STANDARD 14)

set(CMAKE_POSITION_INDEPENDENT_CODE ON)  # apparently necessary to link with OpenDL

set(SOURCE_FILES
        ../../source/CF/CFArray.cpp
        ../../source/CF/CFAttributedString.cpp
        ../../source/CF/CFBoolean.cpp
        ../../source/CF/CFDictionary.cpp
        ../../source/CF/CFMisc.cpp
        ../../source/CF/CFMutableArray.cpp
        ../../source/CF/CFMutableAttributedString.cpp
        ../../source/CF/CFMutableDictionary.cpp
        ../../source/CF/CFMutableString.cpp
        ../../source/CF/CFNumber.cpp
        ../../source/CF/CFObject.cpp
        ../../source/CF/CFString.cpp
        ../../source/CF/CFURL.cpp
        ../../source/AbstractRangeManager.cpp
        ../../source/util.cpp
        )

add_library(cfminimal ${SOURCE_FILES})
