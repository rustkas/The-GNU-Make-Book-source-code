# function notlast(LIST)
notlast = $(wordlist 2, $(words $1), dummy $1)

MY_LIST = a program for directed compilation

$(info The text is "$(MY_LIST)")
$(info The head text is "$(call notlast, $(MY_LIST))")

.PHONY: all
.DEFAULT: all
all: ;
