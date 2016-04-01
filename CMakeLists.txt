# TODO: convert configure.ac to config.h.cmake
# configure_file(${CMAKE_CURRENT_SOURCE_DIR}/config.h.cmake ${CMAKE_CURRENT_BINARY_DIR}/config.h)

include_directories(${gnssrecv_SOURCE_DIR}/ffts)

add_subdirectory(src)


########### install files ###############

#original Makefile.am contents follow:

#AUTOMAKE_OPTIONS = foreign
#SUBDIRS = src tests
#EXTRA_DIST=COPYRIGHT ffts.pc.in build_iphone.sh build_android.sh
#ACLOCAL_AMFLAGS = -Im4
#
#pkgconfigdir = $(libdir)/pkgconfig
#pkgconfig_DATA = ffts.pc
#
#if ENABLE_JNI
#SUBDIRS += java
#endif
