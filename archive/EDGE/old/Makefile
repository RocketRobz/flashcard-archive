.PHONY: package

export TOPDIR := $(CURDIR)
export BASE   := EDGE/$(shell basename $(CURDIR))
export OUT    := $(TOPDIR)/../../../out
export COMMON := $(TOPDIR)/../../../common-kernels

package: directory EDGE_OS_1.36.zip EDGE_OS_1.37.zip EDGE_OS_1.40.zip EDGE_OS_1.41.zip

directory:
	mkdir -p $(OUT)/$(BASE)

EDGE_OS_1.36.zip: directory
	cd $(TOPDIR)/EDGE_OS_1.36 && zip -r $(OUT)/$(BASE)/$@ *

EDGE_OS_1.37.zip: directory
	cd $(TOPDIR)/EDGE_OS_1.37 && zip -r $(OUT)/$(BASE)/$@ *

EDGE_OS_1.40.zip: directory
	cd $(TOPDIR)/EDGE_OS_1.40 && zip -r $(OUT)/$(BASE)/$@ *

EDGE_OS_1.41.zip: directory
	cd $(TOPDIR)/EDGE_OS_1.41 && zip -r $(OUT)/$(BASE)/$@ *
