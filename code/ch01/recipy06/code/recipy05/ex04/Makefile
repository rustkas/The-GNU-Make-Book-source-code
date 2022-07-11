TRUE = true
FALSE =
and = $(if $1, $(if $2,T))

$(info or)
$(info true,   true: $(call and, TRUE, TRUE))
$(info true,  false: $(call and, TRUE, FALSE))
$(info false,  true: $(call and, FALSE, TRUE))
$(info false,  true: $(call and, FALSE, TRUE))
$(info false, false: $(call and, FALSE, FALSE))

.PHONY: all
.DEFAULT: all
all: ;