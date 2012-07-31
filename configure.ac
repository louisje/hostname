#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.63])
AC_INIT([hostname], [3.06ubuntu1-1], [louisje@gmail.com])
AM_INIT_AUTOMAKE
AC_CONFIG_SRCDIR([hostname.c])
AC_CONFIG_HEADERS([config.h])

# Checks for programs.
AC_PROG_CC
AC_PROG_INSTALL
AC_PROG_LN_S

# Checks for libraries.
# FIXME: Replace `main' with a function in `-lnsl':
AC_CHECK_LIB([nsl], [getnameinfo])

# Checks for header files.
AC_CHECK_HEADERS([arpa/inet.h netdb.h netinet/in.h stdlib.h string.h unistd.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_TYPE_SIZE_T

# Checks for library functions.
AC_FUNC_MALLOC
AC_FUNC_REALLOC
AC_CHECK_FUNCS([gethostbyname gethostname memchr memset sethostname strchr strdup strerror])

AC_CONFIG_FILES([Makefile])
AC_OUTPUT
