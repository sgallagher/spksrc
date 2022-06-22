PKG_NAME = http-parser
PKG_VERS = 2.9.4
PKG_EXT = tar.gz
PKG_DIST_NAME = v$(PKG_VERS).$(PKG_EXT)
PKG_DIST_SITE = https://github.com/nodejs/http-parser/archive
PKG_DIST_FILE = $(PKG_NAME)-$(PKG_VERS).$(PKG_EXT)
PKG_DIR = $(PKG_NAME)-$(PKG_VERS)

DEPENDS =

HOMEPAGE = https://github.com/nodejs/http-parser
COMMENT  = HTTP request/response parser for C
LICENSE  = MIT

POST_EXTRACT_TARGET = http_parser_post_extract

include ../../mk/spksrc.cross-meson.mk

.PHONY: http_parser_post_extract
http_parser_post_extract:
	cp -f meson.build $(WORK_DIR)/$(PKG_DIR)/
	sed -i "s/__VERSION__/3.0.0/g" $(WORK_DIR)/$(PKG_DIR)/meson.build

