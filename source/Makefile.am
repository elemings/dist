
bin_PROGRAMS = myprog

myprog_SOURCES = myprog.c
myprog_CPPFLAGS = -I$(top_srcdir)/include
myprog_LDADD = $(top_builddir)/library/libmy.la

$(top_builddir)/library/libmy.la:
	cd $(top_builddir)/library && $(MAKE) $(AM_MAKEFLAGS)

maintainer-clean-local:
	-rm -f Makefile.in

