HAVE_CURL := $(shell which curl)
HAVE_CURL2 := $(shell which curl2)


$(info Does system have curl tool?)
ifndef HAVE_CURL
$(error curl is missing)
else
$(info Yes. curl is here.)
endif

$(info Does system have curl2 tool?)
ifndef HAVE_CURL2
$(error curl2 is missing)
else
$(info Yes. curl2 is here.)
endif

.PHONY: all
.DEFAULT: all
all: ; $(info)