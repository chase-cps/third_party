###############################################################################
# CMake file for the third party dependencies for CHASE.
# @author Michele Lora
###############################################################################
cmake_minimum_required (VERSION 3.10)
set(CMAKE_BUILD_TYPE DEBUG)
set(CMAKE_C_FLAGS_DEBUG "-O0 -Wall -Wextra -pedantic -ggdb -fPIC")
set(CMAKE_C_FLAGS_RELEASE "-O3 -fPIC")
set(CMAKE_CXX_FLAGS_DEBUG "-O0 -Wall -Wextra -pedantic -ggdb -fPIC")
set(CMAKE_CXX_FLAGS_RELEASE "-O3  -fPIC")
set(CMAKE_INSTALL_PREFIX $ENV{CHASE_INSTALL_DIR} CACHE PATH "Install top-level directory" FORCE)

project(THIRD_PARTY_CHASE CXX)

add_subdirectory(antlr4)

