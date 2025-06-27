cmake_minimum_required (VERSION 2.6)
project (BitBufferCpp)

add_library(BitBufferCpp src/bit_buffer.cpp)
# Turn on -fPIC so this library can be linked by shared libraries.
set_target_properties(BitBufferCpp PROPERTIES POSITION_INDEPENDENT_CODE TRUE)

target_include_directories(BitBufferCpp PUBLIC ${PROJECT_SOURCE_DIR}/src)
