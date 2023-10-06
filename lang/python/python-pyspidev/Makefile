#
# Copyright (C) 2023 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-pyspidev
PKG_VERSION:=3.5
PKG_RELEASE:=1

PYPI_NAME:=spidev
PKG_HASH:=8a7f5c289f161ea2ac4697fa8a10918232c990678dd0053084b3c43b1363910d

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Nicolò Veronese <nicveronese@gmail.com>

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-pyspidev
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Module to access spidev devices
  URL:=https://github.com/doceme/py-spidev
  DEPENDS:=+python3-base +python3-setuptools
endef

define Package/python3-pyspidev/description
This project contains a python module for interfacing
 with SPI devices from user space via the
 spidev linux kernel driver.
endef

$(eval $(call Py3Package,python3-pyspidev))
$(eval $(call BuildPackage,python3-pyspidev))
$(eval $(call BuildPackage,python3-pyspidev-src))
