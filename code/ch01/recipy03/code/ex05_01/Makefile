export FOO=bar

.PHONY: all

all: first second third fourth fifth

first: export FOO=just for all
first: ; @echo FOO is $$FOO

second: ; @echo FOO is $$FOO

third: export FOO=
third: ; @echo FOO is $$FOO

fourth: ; @echo FOO is $$FOO

fifth: ; @export FOO=foo; echo FOO is $$FOO