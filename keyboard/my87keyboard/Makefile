# 此工程的根目录
ROOT_DIR := ../..

# 特殊目录控制
# SDK_ROOT := /var/nrf52/nRF52_SDK
# TEMPLATE_PATH := /var/nrf52/template


# 配置文件文件名
CONFIG_H = config.h
CONFIG_H_DIR = .
SRC_FILES += keymap_plain.c

include ./rules.mk

########## STOP HERE ##########
# 除非你知道下面这些配置项是干什么的，否则不要去动它

INC_FOLDERS += .

APP_MAIN_DIR := $(ROOT_DIR)/application/main
TMK_CORE_DIR := $(ROOT_DIR)/tmk/tmk_core
USB_SOURCE_DIR := $(ROOT_DIR)/usb

APP_PROJ_DIR := $(APP_MAIN_DIR)/project
APP_SRC_DIR := $(APP_MAIN_DIR)/src

all: default ch554

include $(APP_PROJ_DIR)/kbd.mk
include $(USB_SOURCE_DIR)/usb.mk
