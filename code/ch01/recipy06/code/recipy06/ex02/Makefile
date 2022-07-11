lastword = $(if $1,$(word $(words $1),$1))

MY_LIST = a program for directed compilation

$(info The text is "$(MY_LIST)")
$(info The last word is "$(call lastword,$(MY_LIST))")

.PHONY: all
.DEFAULT: all
all: ;
