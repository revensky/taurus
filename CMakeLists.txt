cmake_minimum_required(VERSION 3.22.1)

project(Taurus CXX)
project(Taurus VERSION 0.1.0)
project(Taurus HOMEPAGE_URL https://github.com/revensky/taurus-learner.git)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

set(CMAKE_CXX_COMPILER clang++)
set(CMAKE_CXX_FLAGS_INIT "-Wall")
set(CMAKE_CXX_FLAGS_DEBUG_INIT "-g")
set(CMAKE_CXX_FLAGS_MINSIZEREL_INIT "-Os -DNDEBUG")
set(CMAKE_CXX_FLAGS_RELEASE_INIT "-O3 -DNDEBUG")
set(CMAKE_CXX_FLAGS_RELWITHDEBINFO_INIT "-O2 -g")

set(MAIN_FILE ${CMAKE_CURRENT_SOURCE_DIR}/src/taurusc.cpp)

add_executable(taurusc ${MAIN_FILE})
