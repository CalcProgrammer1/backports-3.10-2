# common
obj-$(CPTCFG_IWLWIFI)	+= iwlwifi.o
iwlwifi-objs		+= iwl-io.o
iwlwifi-objs		+= iwl-drv.o
iwlwifi-objs		+= iwl-debug.o
iwlwifi-objs		+= iwl-notif-wait.o
iwlwifi-objs		+= iwl-eeprom-read.o iwl-eeprom-parse.o
iwlwifi-objs		+= iwl-phy-db.o iwl-nvm-parse.o
iwlwifi-objs		+= pcie/drv.o pcie/rx.o pcie/tx.o pcie/trans.o
iwlwifi-objs		+= iwl-1000.o iwl-2000.o iwl-5000.o iwl-6000.o iwl-7000.o

iwlwifi-$(CPTCFG_IWLWIFI_DEVICE_TRACING) += iwl-devtrace.o
iwlwifi-$(CPTCFG_IWLWIFI_DEVICE_TESTMODE) += iwl-test.o

ccflags-y += -D__CHECK_ENDIAN__ -I$(src)


obj-$(CPTCFG_IWLDVM)	+= dvm/
obj-$(CPTCFG_IWLMVM)	+= mvm/

CFLAGS_iwl-devtrace.o := -I$(src)
