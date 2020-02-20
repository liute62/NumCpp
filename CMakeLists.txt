PROJECT(Numpy)

if(CPPBUILD)
  include("cppbuild.cmake")
  return()
endif()

cmake_minimum_required(VERSION 2.6.2)

if (COMMAND set_up_hermetic_build)
  set_up_hermetic_build()
endif()



# Where Numpy's .h files can be found.
include_directories(
  ${Numpy_SOURCE_DIR}/include
  ${Numpy_SOURCE_DIR}/include/NumCpp)
