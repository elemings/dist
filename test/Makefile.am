
check_PROGRAMS = \
        test01
TESTS = \
        test01
test01_SOURCES = \
	test01.c
test01_CPPFLAGS = \
	-I$(top_srcdir)/include

LDADD = $(top_builddir)/library/libmy.la
AM_LDFLAGS = -export-dynamic
$(top_builddir)/library/libmy.la:
	cd $(top_builddir)/library && $(MAKE) $(AM_MAKEFLAGS)

maintainer-clean-local:
	-$(RM) Makefile.in

