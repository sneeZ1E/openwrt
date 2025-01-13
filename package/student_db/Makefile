include $(TOPDIR)/rules.mk

PKG_NAME:=student_db
PKG_RELEASE:=1

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=git@github.com:sneeZ1E/student-db.git
PKG_SOURCE_DATE:=2024-12-12
PKG_SOURCE_VERSION:=afb9e6c
PKG_MIRROR_HASH:=skip

PKG_MAINTAINER:=Martins Lacis <martins.laacis13@gmail.com>

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
	SECTION:=RTU
	CATEGORY:=RTU
	DEPENDS:=+libc
	TITLE:=Student database write then read app
endef

define Package/$(PKG_NAME)/description
CLI application that allows to enter student data and read it 
afterwards.
endef

define Package/$(PKG_NAME)/install
	$(INSTALL_DIR) $(1)/usr/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/student_db $(1)/usr/bin
endef

$(eval $(call BuildPackage,$(PKG_NAME)))