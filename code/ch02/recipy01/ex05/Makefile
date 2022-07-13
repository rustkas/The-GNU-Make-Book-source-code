ifdef TRACE
.PHONY: _trace _value
_trace: ; @$(MAKE) --no-print-directory TRACE= \
$(TRACE)='$$(warning TRACE $(TRACE))$(shell $(MAKE) TRACE=$(TRACE) _value)'
_value: ; @echo '$(value $(TRACE))'
endif

all: FOO=foo
all: a
all: ; @echo $(FOO)
a: ; @echo $(FOO)

