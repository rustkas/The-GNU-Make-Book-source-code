include gmsl

APP_NAME:=cat
findpath = $(call first,$(call map,wildcard,$(call addsuffix,/$1,$(call split,:,$(PATH)))))

#$(info PATH = $(PATH))

$(info $(APP_NAME) PATH = $(call findpath,$(APP_NAME)))

.PHONY: all

all: ; @true