include gmsl

ifcase = $(call seq,$(call lc,$1),$(call lc,$2))

DEBUG := yes

CPPFLAGS :=
CPPFLAGS += $(if $(call ifcase,$(DEBUG),yes),-DDEBUG,)

$(info CPPFLAGS = $(CPPFLAGS))

.PHONY: all

all: ; @true