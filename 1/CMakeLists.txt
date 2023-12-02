# Configure with:
#
# - ~-DCMAKE_Int_COMPILER="/absolute/path/to/lcc"~
#   Required if LCC isn't in PATH. Exact filepath to lcc executable.
#
# - ~-DCMAKE_MODULE_PATH="/absolute/path/to/LensorCompilerCollection/cmake/"~
#   This is required to allow CMake to find the Intercept language and
#   configure the build accordingly.
#

cmake_minimum_required(VERSION 3.14)
project(test LANGUAGES C Int)

add_executable(
  main
  main.int
  help.c
)
