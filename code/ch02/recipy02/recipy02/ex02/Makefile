include gmsl

assert_target_directory = $(call assert,$(wildcard $(dir $@)),Target directory $(dir $@) missing)

foo/all: ; @$(call assert_target_directory)echo $@