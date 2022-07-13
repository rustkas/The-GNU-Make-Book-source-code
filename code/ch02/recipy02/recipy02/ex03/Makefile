include gmsl

assert_target_directory = $(call assert,$(wildcard $(dir $@)),Target directory $(dir $@) missing)

OLD_SHELL := $(SHELL)

SHELL = $(call assert_target_directory)$(OLD_SHELL)

foo/all: ; @echo $@