
########### next target ###############

SET(test_SRCS
   test.c
)

add_executable(test ${test_SRCS})

target_link_libraries(test ffts)


########### install files ###############




#original Makefile.am contents follow:

#
#noinst_PROGRAMS = test
#test_SOURCES = test.c
#test_LDADD = $(top_builddir)/src/libffts.la
