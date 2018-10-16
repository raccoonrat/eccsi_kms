#ECCSIDIR = @ECCSIDIR@
AUTOMAKE_OPTIONS = std-options subdir-objects

lib_LTLIBRARIES= libkmsdb.la

libkmsdb_la_SOURCES = kmsdb.c
libkmsdb_la_CFLAGS = -I$(top_srcdir)/include -I${ECCSIDIR}/include 
libkmsdb_la_LIBADD = -lm -lrt -lpthread -ldl
libkmsdb_la_LDFLAGS = -version-info 1:0:1

