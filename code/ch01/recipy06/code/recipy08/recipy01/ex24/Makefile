MAKE_MIN_VERSION := 4.0

MAKE_OK_VERSION := $(filter $(need),$(firstword $(sort $(MAKE_VERSION) $(need))))

ifdef MAKE_OK_VERSION
$(error your version of make is old)
endif

.PHONY: all
.DEFAULT_GOAL = all

is_feature = $(if $(filter $1,$(.FEATURES)),T)

#$(info $(sort $(.FEATURES)))
#$(info)


$(if $(call is_feature, guile), $(if $(guile (access? "foo.c" R_OK)),$(info foo.c exists)))

	
all: ; @true