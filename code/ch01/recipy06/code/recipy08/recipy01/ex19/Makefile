MAKE_MIN_VERSION := 3.82

MAKE_OK_VERSION := $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))

ifdef MAKE_OK_VERSION
$(error your version of make is old)
endif

.PHONY: all
.DEFAULT_GOAL = all

# set Tab as a recipy prefix
.RECIPEPREFIX =	
.ONESHELL:

all: foo.o
	
	
DEBUG=0
foo.o: private DEBUG=1
foo.o: foo.c
	@echo DEBUG is $(DEBUG) for $@
foo.c: foo.in
	@echo DEBUG is $(DEBUG) for $@