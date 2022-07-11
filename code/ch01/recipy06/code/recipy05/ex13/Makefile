assert-command-present = $(if $(shell which $1),,$(error '$1' missing and needed for this build))

.PHONY: all
.DEFAULT: all
all: ; @echo Do all...
download: export _check = $(call assert-command-present,curly)
download: ; @echo Download stuff...
