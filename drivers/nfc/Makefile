#
# Makefile for nfc devices
#

obj-$(CONFIG_PN544_NFC)		+= pn544.o
ifeq ($(CONFIG_MACH_FIND7OP),y)
obj-$(CONFIG_PN544_NFC_OPPO)	+= pn544-oppo_find7op.o
else ifeq ($(CONFIG_MACH_N3),y)
obj-$(CONFIG_PN544_NFC_OPPO)	+= pn544-oppo_n3.o
obj-$(CONFIG_PN544_NFC_OPPO)	+= p61-oppo_n3.o
else
obj-$(CONFIG_PN544_NFC_OPPO)	+= pn544-oppo.o
endif
obj-$(CONFIG_NFC_PN533)		+= pn533.o
obj-$(CONFIG_NFC_WILINK)	+= nfcwilink.o
obj-$(CONFIG_NFC_QNCI)		+= nfc-nci.o

ccflags-$(CONFIG_NFC_DEBUG) := -DDEBUG
