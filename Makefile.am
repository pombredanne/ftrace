lib_ftracedir = $(libdir)/ftrace
lib_ftrace_PROGRAMS = libftrace.so
libftrace_so_SOURCES = libftrace.c prototype.c
libftrace_so_CFLAGS = -fPIC -shared
libftrace_so_LDADD = -ldwarf
bin_PROGRAMS = ftrace
noinst_PROGRAMS = ftrace-test
ftrace_SOURCES = ftrace.c
ftrace_test_SOURCES = ftrace-test.c
ftrace_test_CFLAGS = -g -O0 -finstrument-functions
ftrace_test_LDADD = -lpthread
man_MANS = ftrace.1
EXTRA_DIST = $(man_MANS) libftrace.h prototype.h
