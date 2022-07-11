MAKE_MIN_VERSION := 4.0

MAKE_OK_VERSION := $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))

ifdef MAKE_OK_VERSION
$(error your version of make is old)
endif

.PHONY: all
.DEFAULT_GOAL = all

all: part-one part-two

part-one: part-three
	@echo Make $@

part-two:
	@echo Make $@

part-three:
	@echo Make $@