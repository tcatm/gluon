# Copyright (C) 2013 Nils Schneider <nils at nilsschneider.net>
# This is free software, licensed under the Apache 2.0 license.

include $(TOPDIR)/rules.mk

PKG_NAME:=gluon-luci-autoupdater
PKG_VERSION:=0.1
PKG_RELEASE:=1

PKG_BUILD_DIR := $(BUILD_DIR)/$(PKG_NAME)

include $(INCLUDE_DIR)/package.mk

define Package/gluon-luci-autoupdater
  SECTION:=gluon
  CATEGORY:=Gluon
  TITLE:=Luci module for gluon-autoupdater
  DEPENDS:=+gluon-luci-admin +gluon-autoupdater
endef

define Package/gluon-luci-autoupdater/description
	Luci module for gluon-autoupdater
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/gluon-luci-autoupdater/install
	$(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,gluon-luci-autoupdater))