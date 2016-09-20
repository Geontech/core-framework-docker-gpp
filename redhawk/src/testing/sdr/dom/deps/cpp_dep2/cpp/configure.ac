AC_INIT(cpp_dep2, 1.0.0)
AM_INIT_AUTOMAKE([nostdinc foreign])
AC_CONFIG_MACRO_DIR([m4])

AC_PROG_CC
AC_PROG_CXX
AC_PROG_INSTALL
LT_INIT([disable-static])

AC_CORBA_ORB
OSSIE_CHECK_OSSIE
RH_SOFTPKG_PREFIX([cpp_dep2],[cpp])

m4_ifdef([AM_SILENT_RULES], [AM_SILENT_RULES([yes])])

# Dependencies
PKG_CHECK_MODULES([REDHAWK], [ossie >= 2.0])
OSSIE_ENABLE_LOG4CXX
AX_BOOST_BASE([1.41])
AX_BOOST_SYSTEM
AX_BOOST_THREAD
AX_BOOST_REGEX

AC_CONFIG_FILES([Makefile cpp_dep2.pc])
AC_OUTPUT