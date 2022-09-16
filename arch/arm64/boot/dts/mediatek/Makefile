# SPDX-License-Identifier: GPL-2.0
dtb-y += mt6833.dtb
dtb-y += mt6833_a14xm_eur_open_00.dtb

ifeq ($(strip $(CONFIG_BUILD_ARM64_DTB_OVERLAY_IMAGE)), y)
dtbo-y += $(addsuffix .dtbo, $(notdir $(subst $\",,$(CONFIG_BUILD_ARM64_DTB_OVERLAY_IMAGE_NAMES))))
endif

always		:= $(dtb-y) $(dtbo-y)
clean-files	:= *.dtb  *.dtbo
