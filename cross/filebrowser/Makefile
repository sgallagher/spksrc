PKG_NAME = filebrowser
PKG_VERS = 2.20.1
PKG_EXT = tar.gz
PKG_DIST_NAME = v$(PKG_VERS).$(PKG_EXT)
PKG_DIST_SITE = https://github.com/filebrowser/$(PKG_NAME)/archive
PKG_DIST_FILE = $(PKG_NAME)-$(PKG_VERS).$(PKG_EXT)
PKG_DIR =  $(PKG_NAME)-$(PKG_VERS)

BUILD_DEPENDS = native/go native/nodejs

HOMEPAGE = https://github.com/filebrowser/filebrowser
COMMENT  = Web File Browser.
LICENSE  = Apache-2.0

PATH := $(WORK_DIR)/../../../native/nodejs/work-native/node/bin:$(PATH)

GO_SRC_DIR = $(WORK_DIR)/$(PKG_NAME)-$(PKG_VERS)
GO_BIN_DIR = $(GO_SRC_DIR)/$(PKG_NAME)
GO_LDFLAGS = -s -w

PRE_COMPILE_TARGET = filebrowser_pre_compile

include ../../mk/spksrc.cross-go.mk

.PHONY: filebrowser_pre_compile
filebrowser_pre_compile:
	@$(RUN) $(MAKE) build-frontend
