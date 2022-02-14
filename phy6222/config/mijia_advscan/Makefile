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

PROGNAME  = $(CONFIG_PHYAPP_MIJIA_ADVSCAN_PROGNAME)
PRIORITY  = $(CONFIG_PHYAPP_MIJIA_ADVSCAN_PRIORITY)
STACKSIZE = $(CONFIG_PHYAPP_MIJIA_ADVSCAN_STACKSIZE)
MODULE    = $(CONFIG_PHYAPP_MIJIA_ADVSCAN)


VPATH = ../../bbb_sdk/example/ble_mesh/mijia_advscan/source:../../bbb_sdk/example/ble_mesh/mijia_advscan/source/bleMesh:../../bbb_sdk/example/ble_mesh/mijia_advscan/source/miot_spec
# simple ble Example

include Make.cflags

CSRCS += app_main.c
CSRCS += bleMesh.c
CSRCS += bleMesh_Main.c
CSRCS += OSAL_bleMesh.c
#CSRCS += appl_sample_example_phylight.c
CSRCS += dongleKey.c

CSRCS += on_action_invoke.c
CSRCS += on_property_get.c
CSRCS += on_property_request.c
CSRCS += on_property_set.c
CSRCS += S_1_DeviceInformation_doGet.c
CSRCS += S_2_Light_doAction.c
CSRCS += S_2_Light_doChange.c
CSRCS += S_2_Light_doGet.c
CSRCS += S_2_Light_doSet.c


MAINSRC = main.c

include $(APPDIR)/Application.mk

