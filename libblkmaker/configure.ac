dnl * Copyright 2012-2014 Luke Dashjr
dnl *
dnl * This program is free software; you can redistribute it and/or modify it
dnl * under the terms of the standard MIT license.  See COPYING for more details.

AC_INIT(
	[libblkmaker],
	[0.5.2],
	[luke_libblkmaker@dashjr.org],
	[libblkmaker],
	[http://github.com/bitcoin/libblkmaker])
AC_CONFIG_AUX_DIR([.])
AC_PREREQ([2.59])
AM_INIT_AUTOMAKE([1.11 -Wall dist-xz foreign])
m4_ifdef([AM_SILENT_RULES], [AM_SILENT_RULES([yes])])

AC_PROG_CC_C99
m4_ifdef([AM_PROG_AR], [AM_PROG_AR])
LT_INIT([disable-shared])

# http://www.gnu.org/software/libtool/manual/html_node/Updating-version-info.html
AC_SUBST([LIBBLKMAKER_SO_VERSION], [6:2:0])
AC_SUBST([LIBBLKMAKER_API_VERSION], [0.1])

AC_CONFIG_FILES([Makefile
	libblkmaker_jansson-${LIBBLKMAKER_API_VERSION}.pc:libblkmaker_jansson.pc.in
])

AC_CHECK_LIB([ws2_32], [strchr])

AC_OUTPUT
