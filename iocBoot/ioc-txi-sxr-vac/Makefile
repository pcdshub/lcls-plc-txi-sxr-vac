IOC_TOP=/reg/g/pcds/epics/ioc/common/ads-ioc/R0.6.1
IOC_INSTANCE_PATH := $(shell pwd)

# Set PRODUCTION_IOC to 1 to move from a testing to a production IOC:
PRODUCTION_IOC := 1

PROJECT_NAME := plc-txi-sxr-vac
PROJECT_PATH := ../../plc-txi-sxr-vac/plc-txi-sxr-vac.tsproj
PLC := txi_sxr_vac

PYTMC_OPTS := 
PREFIX := PLC:TXI:SXR:VAC

# With two $$, as in $$(IOC) below, this will be expanded in the
# environment of st.cmd:
DB_PARAMETERS := 'PREFIX=$(PREFIX):,IOCNAME=$$(IOC),IOC=$$(IOC)'

include $(IOC_TOP)/iocBoot/templates/Makefile.base
