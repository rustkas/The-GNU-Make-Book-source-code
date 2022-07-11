MAKE_MIN_VERSION := 4.0

MAKE_OK_VERSION := $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))

ifdef MAKE_OK_VERSION
$(error your version of make is old)
endif

.PHONY: all
.DEFAULT_GOAL = all

all: one two three four

one two:
	@echo $@ line start
	@sleep 0.1s
	@echo $@ line middle
	@echo $@ line finish

three four:
	@echo $@ line start
	@sleep 0.2s
	@echo $@ line middle
	@echo $@ line finish
	