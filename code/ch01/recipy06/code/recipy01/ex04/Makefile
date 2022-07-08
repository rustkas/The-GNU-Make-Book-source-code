need := 3.8
$(info items: $(MAKE_VERSION) $(need))
$(info sort result: $(sort $(MAKE_VERSION) $(need)))
$(info firstword result: $(firstword $(sort $(MAKE_VERSION) $(need))))

ok = $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))
.PHONY: all
all: ; @echo Make version is $(ok)