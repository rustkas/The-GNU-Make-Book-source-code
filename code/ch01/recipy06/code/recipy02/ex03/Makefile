# Returns T if the requested feature is supported 
# or an empty string if the feature is missing:
is_feature = $(if $(filter $1,$(.FEATURES)),T)
$(info $(origin .FEATURES))

FEATURE_LIST := $(sort $(.FEATURES))
 
.PHONY: all

all: $(FEATURE_LIST)
#	@echo archives are $(if $(call is_feature,archives),,not )available
$(FEATURE_LIST): ; @echo $@ are $(if $(call is_feature,$@),,not )available
#guile: ; @echo $@ are $(if $(call is_feature,$@),,not )available