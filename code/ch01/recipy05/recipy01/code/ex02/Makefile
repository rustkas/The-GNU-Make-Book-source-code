.PHONY: all foo bar baz

VAR = global scope

all: foo bar
all foo bar baz: ; @echo In $@ VAR is $(VAR)

bar: VAR = local scope

bar: baz
