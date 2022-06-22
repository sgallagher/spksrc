PKG_NAME = tang
PKG_VERS = 11
PKG_EXT = tar.gz
PKG_DIST_NAME = v$(PKG_VERS).$(PKG_EXT)
PKG_DIST_SITE = https://github.com/latchset/tang/archive
PKG_DIST_FILE = $(PKG_NAME)-$(PKG_VERS).$(PKG_EXT)
PKG_DIR = $(PKG_NAME)-$(PKG_VERS)

DEPENDS = cross/http-parser \
          cross/jose \
          cross/openssl \
          cross/zlib

HOMEPAGE = https://github.com/latchset/jose
COMMENT  = A server for binding data to network presence
LICENSE  = GPLv3

include ../../mk/spksrc.cross-meson.mk
