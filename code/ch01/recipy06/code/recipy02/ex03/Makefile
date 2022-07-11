# Returns T if the requested feature is supported 
# or an empty string if the feature is missing:
is_feature = $(if $(filter $1,$(.FEATURES)),T)
$(info $(origin .FEATURES))

FEATURE_LIST := $(sort $(.FEATURES) guile)
 
.PHONY: all

all: $(FEATURE_LIST)

$(FEATURE_LIST): ITEM = $@
$(FEATURE_LIST): ; @echo $(ITEM) are $(if $(call is_feature,$(ITEM)),,not )available
