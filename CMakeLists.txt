cmake_minimum_required(VERSION 3.18)

project(XEMBED
  VERSION 0.1.0
  LANGUAGES C
  HOMEPAGE_URL "https://github.com/agate-lang/xembed"
)

include(GNUInstallDirs)

add_executable(xembed
  xembed.c
)

install(
  TARGETS xembed
  RUNTIME DESTINATION "${CMAKE_INSTALL_BINDIR}"
)
