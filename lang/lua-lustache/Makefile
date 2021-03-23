
include $(TOPDIR)/rules.mk

PKG_NAME:=lua-lustache
PKG_SOURCE_VERSION:=c2e7573a1d19e93f5498143d95d9fa705ee512fd
PKG_VERSION:=1.3.1-0
PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://github.com/Olivine-Labs/lustache.git
PKG_SOURCE_PROTO:=git
PKG_SOURCE_SUBDIR:=$(PKG_NAME)-$(PKG_VERSION)

include $(INCLUDE_DIR)/package.mk

define Package/lua-lustache
  SUBMENU:=Lua
  SECTION:=lang
  CATEGORY:=Languages
  TITLE:=Lua-lustache
  DEPENDS:=+lua
endef

define Package/lua-lustache/description
lustache is an implementation of the mustache template system in Lua.

Mustache is a logic-less template syntax. It can be used for HTML, config files, source code - anything. It works by expanding tags in a template using values provided in a hash or object.

We call it "logic-less" because there are no if statements, else clauses, or for loops. Instead there are only tags. Some tags are replaced with a value, some nothing, and others a series of values.
endef

define Build/prepare
endef

define Build/Compile
endef

define Package/lua-lustache/install
	$(INSTALL_DIR) 	$(1)/usr/lib/lua
	$(CP) $(PKG_BUILD_DIR)/src/* $(1)/usr/lib/lua
endef

$(eval $(call BuildPackage,lua-lustache))
