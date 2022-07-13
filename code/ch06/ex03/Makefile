include gmsl

# List containing the desired library version number (maj min rev)
MIN_GMSL_VERSION:=1 1 2

$(info $(if $(call gmsl_compatible,$(MIN_GMSL_VERSION)),GMSL is compatible,Wrong GMSL version))

.PHONY: all

all: ; @true