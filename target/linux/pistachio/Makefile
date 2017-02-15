#
# Copyright (C) 2017 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#
include $(TOPDIR)/rules.mk

ARCH:=mipsel
BOARD:=pistachio
BOARDNAME:=MIPS pistachio
FEATURES:=fpu usb usbgadget targz nand squashfs ubifs audio
CPU_TYPE:=24kc
CPU_SUBTYPE:=24kf
MAINTAINER:=

KERNEL_PATCHVER:=4.9

include $(INCLUDE_DIR)/target.mk

KERNELNAME:=dtbs

DEFAULT_PACKAGES += \
	kmod-leds-gpio kmod-ledtrig-heartbeat \
	kmod-i2c-core kmod-serial-sc16is7xx \
	kmod-sound-pistachio-soc alsa-utils \
	uboot-envtools

$(eval $(call BuildTarget))
