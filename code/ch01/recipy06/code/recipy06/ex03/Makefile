MAKE_MIN_VERSION := 3.81

MAKE_OK_VERSION := $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))

ifdef MAKE_OK_VERSION
$(error your version of make is old)
endif

MY_LIST = a program for directed compilation

$(info The text is "$(MY_LIST)")
$(info The last word is "$(lastword $(MY_LIST))")


.PHONY: all
.DEFAULT: all
all: ;
