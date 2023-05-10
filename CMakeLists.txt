cmake_minimum_required(VERSION 3.22)
cmake_policy(SET CMP0097 NEW)

project(bitcoin VERSION 1.0)

cmake_host_system_information(RESULT OS_NAME QUERY OS_NAME)  # OS_NAME

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
# set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -v")

set(GLOBAL_SOURCE_DIR ${PROJECT_SOURCE_DIR}/src)
set(GLOBAL_INCLUDE_DIR ${PROJECT_SOURCE_DIR}/src)
set(GLOBAL_LIB_DIR ${PROJECT_SOURCE_DIR}/src)

include_directories(${GLOBAL_INCLUDE_DIR})
# link_directories(
#   ${GLOBAL_LIB_DIR}
#   ${GLOBAL_LIB_DIR}/crypto/.libs
# )

