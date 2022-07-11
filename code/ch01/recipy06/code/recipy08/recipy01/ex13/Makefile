MAKE_MIN_VERSION := 3.82

MAKE_OK_VERSION := $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))

ifdef MAKE_OK_VERSION
$(error your version of make is old)
endif

.PHONY: all
.DEFAULT_GOAL = all

sp :=
sp += 
has$(sp)space := variable with space in name
$(info ok)
$(if $(has space), $(info $(has space)), $(info Can't use variable with a space into a name))


all: ; @true