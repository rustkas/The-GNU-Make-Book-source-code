MAKE_MIN_VERSION := 4.0

MAKE_OK_VERSION := $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))

ifdef MAKE_OK_VERSION
$(error your version of make is old)
endif

.PHONY: all
.DEFAULT_GOAL = all

LOG = make.log

$(info Current log content:)
$(info $(file < $(LOG)))
$(info ---- )

all: part-one part-two

part-one: part-three
	@$(file >> $(LOG),$@)
	@echo Make $@

part-two:
	@$(file >> $(LOG),$@)
	@echo Make $@

part-three:
	@$(file >> $(LOG),$@)
	@echo Make $@