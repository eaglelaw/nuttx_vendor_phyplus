############################################################################
# 
#
# Licensed to the Apache Software Foundation (ASF) under one or more
# contributor license agreements.  See the NOTICE file distributed with
# this work for additional information regarding copyright ownership.  The
# ASF licenses this file to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance with the
# License.  You may obtain a copy of the License at
#
#   http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
# License for the specific language governing permissions and limitations
# under the License.
#
############################################################################

include $(APPDIR)/Make.defs

# simple ble! built-in application info

PROGNAME  = $(CONFIG_PHYAPP_MSH_LIGHT_PROGNAME)
PRIORITY  = $(CONFIG_PHYAPP_MSH_LIGHT_PRIORITY)
STACKSIZE = $(CONFIG_PHYAPP_MSH_LIGHT_STACKSIZE)
MODULE    = $(CONFIG_PHYAPP_MSH_LIGHT)

# simple ble Example

include Make.cflags

CSRCS += ../../bbb_sdk/example/ble_peripheral/sbpAdvScan/source/OSAL_SimpleBLEPeripheral.c
CSRCS += ../../bbb_sdk/example/ble_peripheral/sbpAdvScan/source/sbpProfile_ota.c
CSRCS += ../../bbb_sdk/example/ble_peripheral/sbpAdvScan/source/simpleBLEPeripheral.c
CSRCS += ../../bbb_sdk/example/ble_peripheral/sbpAdvScan/source/SimpleBLEPeripheral_Main.c

MAINSRC = ../../bbb_sdk/example/ble_peripheral/sbpAdvScan/main.c

include $(APPDIR)/Application.mk

#clean:
#	@echo 	$(call DELFILE, ../../bbb_sdk/example/ble_peripheral/simpleBlePeripheral/source/*.o)
#	$(call DELFILE, ../../bbb_sdk/example/ble_peripheral/simpleBlePeripheral/source/*.o)
