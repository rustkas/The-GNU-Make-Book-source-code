.PHONY: all foo bar baz

VAR = global scope

all: foo bar
all: ; @echo In $@ VAR is $(VAR)

foo: ; @echo In $@ VAR is $(VAR)

bar: VAR = local scope
bar: baz
bar: ; @echo In $@ VAR is $(VAR)

baz: ; @echo In $@ VAR is $(VAR)