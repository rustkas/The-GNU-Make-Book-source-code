export FOO=bar
$(info $(shell FOO=$(FOO) printenv | grep FOO))

.PHONY: all
all: ; @printenv | grep FOO