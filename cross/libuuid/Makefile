PKG_NAME = libuuid
PKG_REAL_NAME = util-linux
PKG_VERS = 2.37.2
PKG_VERS_MAJOR = $(word 1,$(subst ., ,$(PKG_VERS))).$(word 2,$(subst ., ,$(PKG_VERS)))
PKG_EXT = tar.xz
PKG_DIST_NAME = $(PKG_REAL_NAME)-$(PKG_VERS).$(PKG_EXT)
PKG_DIST_SITE = https://www.kernel.org/pub/linux/utils/$(PKG_REAL_NAME)/v$(PKG_VERS_MAJOR)
PKG_DIR = $(PKG_REAL_NAME)-$(PKG_VERS)

DEPENDS =

HOMEPAGE = https://github.com/karelzak/util-linux
COMMENT  = Random collection of Linux utilities. We use this only to build libuuid out of util-linux.
LICENSE  = GPLv2

GNU_CONFIGURE = 1
CONFIGURE_ARGS  = --without-ncurses --without-python
# We use libuuid only
CONFIGURE_ARGS += --disable-all-programs --enable-libuuid

include ../../mk/spksrc.cross-cc.mk
