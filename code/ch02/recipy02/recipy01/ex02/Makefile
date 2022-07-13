include gmsl

$(foreach o,$(MAKEFLAGS),$(call assert,$(call sne,-i,$o),You can't use the -i option))

ifneq ($(patsubst -%,-,$(firstword $(MAKEFLAGS))),-)
$(call assert,$(call sne,$(patsubst i%,i,$(patsubst %i,i,$(firstword \
$(MAKEFLAGS)))),i),You can't use the -i option)
endif