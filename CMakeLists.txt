# The following lines of boilerplate have to be in your project's
# CMakeLists in this exact order for cmake to work correctly
cmake_minimum_required(VERSION 3.5)


set(HOMEKIT_PATH ${CMAKE_CURRENT_LIST_DIR}/dependencies/esp-homekit-sdk)
# set(IOT_SOLUTION_PATH ${CMAKE_CURRENT_LIST_DIR}/dependencies/esp-iot-solution)

set(EXTRA_COMPONENT_DIRS 
  ${HOMEKIT_PATH}/components
  ${HOMEKIT_PATH}/components/homekit
  ${HOMEKIT_PATH}/examples/common
  ${HOMEKIT_PATH}/components/button)
  # ${IOT_SOLUTION_PATH}/components/general/button)

include($ENV{IDF_PATH}/tools/cmake/project.cmake)
project(hello-world)


