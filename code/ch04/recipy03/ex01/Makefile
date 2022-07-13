
set = $(eval $1 := $2)

FOO := foo
BAR := bar

A := a
B := b
$(call set,FOO,BAR)
$(call set,A,B)

$(info FOO = $(FOO))
$(info A = $(A))

.PHONY: all

all: ; @true