.PHONY: all

FOO=foo
BAR=bar
BAZ=baz
#FOOBAR := $(FOO) $(BAR)
FOOBAR = $(FOO) $(BAR)
FOOBAR += $(BAZ)
BAZ=bazzy

all: $(FOOBAR)

$(FOOBAR): ; @echo $(FOOBAR)