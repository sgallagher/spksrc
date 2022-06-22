PKG_NAME = jansson
PKG_VERS = 2.14
PKG_EXT = tar.gz
PKG_DIST_NAME = v$(PKG_VERS).$(PKG_EXT)
PKG_DIST_SITE = https://github.com/akheron/jansson/archive
PKG_DIST_FILE = $(PKG_NAME)-$(PKG_VERS).$(PKG_EXT)
PKG_DIR = $(PKG_NAME)-$(PKG_VERS)

DEPENDS =

HOMEPAGE = https://harfbuzz.github.io/
COMMENT  = C library for encoding, decoding and manipulating JSON data
LICENSE  = MIT

CMAKE_ARGS  = -DJANSSON_BUILD_DOCS=OFF
CMAKE_ARGS += -DJANSSON_BUILD_SHARED_LIBS=ON

include ../../mk/spksrc.archs.mk
include ../../mk/spksrc.cross-cmake.mk
