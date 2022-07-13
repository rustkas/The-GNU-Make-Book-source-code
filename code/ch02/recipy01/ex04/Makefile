ifdef TRACE
.PHONY: _trace _value
_trace: ; @$(MAKE) --no-print-directory TRACE= \
$(TRACE)='$$(warning TRACE $(TRACE))$(shell $(MAKE) TRACE=$(TRACE) _value)'
_value: ; @echo '$(value $(TRACE))'
endif

X=$(YS) hate $(ZS)
Y=dog
YS=$(Y)$(S)
Z=cat
ZS=$(Z)$(S)
S=s

all: $(YS) $(ZS)
all: ; @echo $(X)

$(YS): ; @echo $(Y) $(Y)
$(ZS): ; @echo $(Z) $(Z)

