cmake_minimum_required(VERSION 3.0)

message( STATUS )
message( STATUS "=============================================================================" )
message( STATUS "== Plugin Build Information                                        ==" )
message( STATUS "=============================================================================" )
message( STATUS "Version:           ${PROJECT_VERSION}")
if (CMAKE_BUILD_TYPE)
    message( STATUS "Build type:        ${CMAKE_BUILD_TYPE}")
endif(CMAKE_BUILD_TYPE)
message( STATUS "Using compiler:    ${CMAKE_CXX_COMPILER_ID} ${CMAKE_CXX_COMPILER_VERSION}" )
message( STATUS "Architecture:      ${CMAKE_CXX_LIBRARY_ARCHITECTURE} / ${CMAKE_LIBRARY_ARCHITECTURE}" )
message( STATUS "System Name:       ${CMAKE_SYSTEM_NAME}" )
message( STATUS "Processor Name:    ${CMAKE_SYSTEM_PROCESSOR}" )
message( STATUS "Using Qt:          ${Qt5_VERSION}" )
message( STATUS "                     [at ${Qt5_DIR}]" )
message( STATUS "Installing to:     ${CMAKE_INSTALL_PREFIX}" )
message( STATUS "  " )
message( STATUS "Environment:" )
message( STATUS "CMAKE_INSTALL_BINDIR:       ${CMAKE_INSTALL_BINDIR}" )
message( STATUS "CMAKE_CURRENT_BINARY_DIR:   ${CMAKE_CURRENT_BINARY_DIR}" )
message( STATUS "CMAKE_BINARY_DIR:           ${CMAKE_BINARY_DIR}" )
message( STATUS "=============================================================================" )
message( STATUS )

include_directories(.)

add_subdirectory(UCD_PWA_Browser)
