export FOO=bar
$(info $(shell printenv | grep FOO))

.PHONY: all
all: ; @printenv | grep FOO