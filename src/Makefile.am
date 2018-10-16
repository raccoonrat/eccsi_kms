AUTOMAKE_OPTIONS = foreign
CFLAGS= @CFLAGS@ -I$(top_srcdir)/include -I${ECCSIDIR}/include -DDEBUG -g
#CFLAGS= @CFLAGS@ -I$(top_srcdir)/include -I${ECCSIDIR}/include  -I${EVDIR}/include
bin_PROGRAMS = kms

kms_SOURCES = kms.c kmsMenu.c  kmsParameters.c
kms_CFLAGS = ${CFLAGS}
#kms_LDADD = ../lib/libtux_ztdh.la -levent -lpthread
kms_LDADD = -L/usr/lib/x86_64-linux-gnu  -lssl -lcrypto \
	${ECCSIDIR}/lib/libesprng.la ${ECCSIDIR}/lib/libesdata.la ${ECCSIDIR}/lib/libescrypt.la ../lib/libkmsdb.la


