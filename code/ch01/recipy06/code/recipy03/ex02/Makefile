T := true
eval_available :=
$(eval eval_available = T)
#$(eval eval_available := true)

ifneq ($(eval_available),T)
$(error This makefile only works with a Make program that support $$(eval))
endif

.PHONY: all

all: ; $(info $(eval_available))