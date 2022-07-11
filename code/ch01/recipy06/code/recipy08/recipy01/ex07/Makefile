MAKE_MIN_VERSION := 3.81

MAKE_OK_VERSION := $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))

ifdef MAKE_OK_VERSION
$(error your version of make is old)
endif

.PHONY: all fail fail1 fail2
.DEFAULT_GOAL = all

fail: ; $(error wrong)
fail1: ; $(error wrong)
fail2: ; $(error wrong)
all:
	$(info right)
	@true


