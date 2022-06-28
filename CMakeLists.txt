cmake_minimum_required(VERSION 3.8)

project (md5)

message(STATUS "This is BINARY dir " ${CMAKE_BINARY_DIR})
message(STATUS "This is SOURCE dir " ${CMAKE_SOURCE_DIR})

add_subdirectory(src bin)

# ----------------------------------------------------------------------------
# package information
set (CPACK_PACKAGE_VERSION_MAJOR    1)
set (CPACK_PACKAGE_VERSION_MINOR    2)
set (CPACK_PACKAGE_VERSION_PATCH    3)
set (CPACK_PACKAGE_CONTACT          "lsc")
set (CPACK_GENERATOR                "lsc")
set (CPACK_PACKAGING_INSTALL_PREFIX "/home/lsc/md5")

include (CPack)

