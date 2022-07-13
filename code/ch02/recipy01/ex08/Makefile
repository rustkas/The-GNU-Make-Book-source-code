OLD_SHELL := $(SHELL)
SHELL = $(warning Building $@)$(OLD_SHELL)

.PHONY: all
all: foo.o bar
bar: ; @touch $@