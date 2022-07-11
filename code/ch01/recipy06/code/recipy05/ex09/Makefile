
have_native_and := $(and T,T)
have_native_or := $(or T,T)

ifneq ($(have_native_and),T)
and = $(if $1,$(if $2,T))
endif
ifneq ($(have_native_or),T)
or = $(if $1$2,T)
endif

$(info This will be T: $(call and,T,T))

.PHONY: all
.DEFAULT: all
all: ; $(info)