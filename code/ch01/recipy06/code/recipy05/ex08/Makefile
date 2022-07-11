
have_native_and := $(and T,T)
have_native_or := $(or T,T)

$(info Have native AND?)
$(if $(call have_native_and), \
	$(info Yes. We have AND.), \
	$(info No. We have not AND.))


$(info Have native OR?)
$(if $(call have_native_or), \
	$(info Yes. We have OR.), \
	$(info No. We have not OR.))


.PHONY: all
.DEFAULT: all
all: ; $(info)