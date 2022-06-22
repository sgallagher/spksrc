PKG_NAME = jose
PKG_VERS = 11
PKG_EXT = tar.gz
PKG_DIST_NAME = v$(PKG_VERS).$(PKG_EXT)
PKG_DIST_SITE = https://github.com/latchset/jose/archive
PKG_DIST_FILE = $(PKG_NAME)-$(PKG_VERS).$(PKG_EXT)
PKG_DIR = $(PKG_NAME)-$(PKG_VERS)

DEPENDS = cross/jansson \
          cross/openssl \
          cross/zlib

HOMEPAGE = https://github.com/latchset/jose
COMMENT  = C-language implementation of the Javascript Object Signing and Encryption standards.
LICENSE  = Apache 2.0

#include ../../mk/spksrc.archs.mk
include ../../mk/spksrc.cross-meson.mk
