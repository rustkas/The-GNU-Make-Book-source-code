MAKE_MIN_VERSION := 3.82

MAKE_OK_VERSION := $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))

ifdef MAKE_OK_VERSION
$(error your version of make is old)
endif

.PHONY: all
.DEFAULT_GOAL = all
.RECIPEPREFIX = >

all:
> @echo Making all