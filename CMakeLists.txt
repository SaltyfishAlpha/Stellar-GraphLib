cmake_minimum_required(VERSION 3.19 FATAL_ERROR)

project( StellarGL )

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(BUILD_SHARED_LIBS OFF)

# ---- Include guards ----
if(PROJECT_SOURCE_DIR STREQUAL PROJECT_BINARY_DIR)
  message(
    FATAL_ERROR
      "In-source builds not allowed. Please make a new directory (called a build directory) and run CMake from there."
  )
endif()

set(ROOT_DIR "${CMAKE_CURRENT_SOURCE_DIR}")

add_subdirectory(engine)