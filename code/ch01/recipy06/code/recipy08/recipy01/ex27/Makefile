MAKE_MIN_VERSION := 4.0

MAKE_OK_VERSION := $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))

ifdef MAKE_OK_VERSION
$(error your version of make is old)
endif

.PHONY: all
.DEFAULT_GOAL = all

CURRENTLY != date

$(info $(CURRENTLY))

CURRENTLY2 ::= $(shell sleep 1s;date)

$(info $(CURRENTLY2))

$(info $(CURRENTLY))

all: ; @true
