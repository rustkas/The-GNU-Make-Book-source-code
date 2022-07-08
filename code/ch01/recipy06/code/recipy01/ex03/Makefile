need := 3.8
TMP_MAKE_VERSION := 3.79.1
$(info items: $(TMP_MAKE_VERSION) $(need))
$(info sort result: $(sort $(TMP_MAKE_VERSION) $(need)))
$(info firstword result: $(firstword $(sort $(TMP_MAKE_VERSION) $(need))))

ok = $(filter $(need),$(firstword $(sort $(TMP_MAKE_VERSION) $(need))))
.PHONY: all
all: ; @echo Make version is $(ok)