# Returns T if the requested feature is supported 
# or an empty string if the feature is missing:
is_feature = $(if $(filter $1,$(.FEATURES)),T)

FEATURE_LIST := $(sort $(.FEATURES) guile) 
 
.PHONY: all

all: $(FEATURE_LIST) guile
#	@echo archives are $(if $(call is_feature,archives),,not )available

$(FEATURE_LIST): ITEM = $@
$(FEATURE_LIST): ; @echo $(ITEM) are $(if $(call is_feature,$(ITEM)),,not )available
#guile: ; @echo $@ are $(if $(call is_feature,$@),,not )available