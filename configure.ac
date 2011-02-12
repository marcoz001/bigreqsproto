AC_PREREQ([2.60])
AC_INIT([BigReqsProto], [1.1.1],
        [https://bugs.freedesktop.org/enter_bug.cgi?product=xorg])
AM_INIT_AUTOMAKE([foreign dist-bzip2])
AM_MAINTAINER_MODE

# Require xorg-macros minimum of 1.11 for XORG_WITH_XSLTPROC
m4_ifndef([XORG_MACROS_VERSION],
          [m4_fatal([must install xorg-macros 1.11 or later before running autoconf/autogen])])
XORG_MACROS_VERSION(1.11)
XORG_DEFAULT_OPTIONS
XORG_ENABLE_SPECS
XORG_WITH_XMLTO(0.0.20)
XORG_WITH_FOP
XORG_WITH_XSLTPROC
XORG_CHECK_SGML_DOCTOOLS(1.5)

AC_OUTPUT([Makefile
           specs/Makefile
           bigreqsproto.pc])
