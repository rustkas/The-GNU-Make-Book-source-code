MAKE_MIN_VERSION := 4.0

MAKE_OK_VERSION := $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))

ifdef MAKE_OK_VERSION
$(error your version of make is old)
endif

.PHONY: all
.DEFAULT_GOAL = all

LIST_FILES = $(shell echo ok)


ifeq ($(.SHELLSTATUS), $(0))
$(info Result is success)
endif


all : ; @true