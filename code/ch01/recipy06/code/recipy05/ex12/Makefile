assert-command-present = $(if $(shell which $1),,$(error '$1' missing and needed for this build))

$(info Does system have curl tool?)
$(if $(call assert-command-present,curl), \
		$(error curl is missing), $(info Yes. The system has curl tool.))

$(info Does system have curly tool?)
$(if $(call assert-command-present,curly), \
		$(error curly is missing), $(info Yes. The system has curly tool.))

.PHONY: all
.DEFAULT: all
all: ; $(info)