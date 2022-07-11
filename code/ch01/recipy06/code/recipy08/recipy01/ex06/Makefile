MAKE_MIN_VERSION := 3.81

MAKE_OK_VERSION := $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))

ifdef MAKE_OK_VERSION
$(error your version of make is old)
endif

has-order-only := $(filter order-only,$(.FEATURES))

ifdef has-order-only
$(info make has "order-only" feature)
endif

.PHONY: all

all: ; @true
