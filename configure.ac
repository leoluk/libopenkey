dnl Process this file with autoconf to produce a configure script.

AC_PREREQ(2.59)
AC_INIT(libopenkey, 0.2)
AC_PROG_CC

AC_CANONICAL_SYSTEM

dnl Initialize automake
AM_INIT_AUTOMAKE

dnl this allows us specify individual liking flags for each target
AM_PROG_CC_C_O 
AC_PROG_CC_C99

dnl Initialize Libtool
LT_INIT

dnl Check if Libtool is present
dnl Libtool is used for building share libraries 
AC_PROG_LIBTOOL

PKG_CHECK_MODULES([DEPS], [libnfc >= 1.7.0 libfreefare >= 0.3.5 uuid])

AM_PATH_LIBGCRYPT

AC_CONFIG_FILES(Makefile
                examples/Makefile
                tools/Makefile
                libopenkey/Makefile
                include/Makefile)
AC_OUTPUT