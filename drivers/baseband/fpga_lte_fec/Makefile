# SPDX-License-Identifier: BSD-3-Clause
# Copyright(c) 2019 Intel Corporation

include $(RTE_SDK)/mk/rte.vars.mk

# library name
LIB = librte_pmd_fpga_lte_fec.a

# build flags
CFLAGS += -DALLOW_EXPERIMENTAL_API
CFLAGS += -O3
CFLAGS += $(WERROR_FLAGS)
LDLIBS += -lrte_eal -lrte_mbuf -lrte_mempool -lrte_ring
LDLIBS += -lrte_bbdev
LDLIBS += -lrte_pci -lrte_bus_pci

# versioning export map
EXPORT_MAP := rte_pmd_bbdev_fpga_lte_fec_version.map

# library version
LIBABIVER := 1

# library source files
SRCS-$(CONFIG_RTE_LIBRTE_PMD_FPGA_LTE_FEC) += fpga_lte_fec.c

# export include files
SYMLINK-$(CONFIG_RTE_LIBRTE_PMD_FPGA_LTE_FEC)-include += fpga_lte_fec.h

include $(RTE_SDK)/mk/rte.lib.mk
