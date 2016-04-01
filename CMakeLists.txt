configure_file(${CMAKE_CURRENT_SOURCE_DIR}/config.h.cmake ${CMAKE_CURRENT_BINARY_DIR}/config.h)

add_subdirectory(src)
add_subdirectory(tests)


########### install files ###############

install(FILES  ffts.pc DESTINATION )



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
