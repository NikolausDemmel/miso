cmake_minimum_required(VERSION 2.8)

project( miso )

set(miso_sources 
	include/miso/miso.h
    miso.cpp
)

add_executable( test_miso ${miso_sources})

target_include_directories( test_miso PUBLIC include )

set_property(TARGET test_miso PROPERTY CXX_STANDARD 11)

