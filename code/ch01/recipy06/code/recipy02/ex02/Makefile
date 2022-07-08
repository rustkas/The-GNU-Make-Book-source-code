has_features = $(if $(filter default, $(origin .FEATURES)), $(if $(.FEATURES), T))

# Returns T if the requested feature is supported 
# or an empty string if the feature is missing:
is_feature = $(if $(call has_features), $(if $(filter $1, $(.FEATURES)), T))

FEATURE_LIST := $(sort $(.FEATURES))
 
.PHONY: all

all: $(FEATURE_LIST)

$(FEATURE_LIST): ; @echo $@ are $(if $(call is_feature,$@), , not )available
